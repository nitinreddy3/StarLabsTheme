sassc = find_program('sassc')

gtk3_dir = join_paths(theme_dir, 'gtk-3.0')
gtk3_asset_dir = join_paths(gtk3_dir, 'assets')

# theme sources .scss files
gtk3_scss_sources = [
  'gtk-dark',
  'gtk',
]


# Dependencies of the files that need to be compiled
gtk3_scss_dependencies = [
  'sass/_starlabs.scss',
  'sass/_functions.scss',
  'sass/functions/_checkradio.scss',
  'sass/functions/_dialog_window.scss',
  'sass/functions/_font-size.scss',
  'sass/functions/_switch.scss',
  'sass/functions/_entries.scss',
  'sass/functions/_header.scss',
  'sass/functions/_undershoot.scss',
  'sass/functions/_clickable.scss',
  'sass/functions/_fill.scss',
  'sass/functions/_overshoot.scss',
  'sass/functions/_general.scss',
  'sass/_src.scss',
  'sass/src/_alpha.scss',
  'sass/src/_base.scss',
  'sass/src/_apps.scss',
  'sass/src/_button.scss',
  'sass/src/_calendar.scss',
  'sass/src/_checkradio.scss',
  'sass/src/_colorchooser.scss',
  'sass/src/_comboboxes.scss',
  'sass/src/_decoration.scss',
  'sass/src/_dialog.scss',
  'sass/src/_emoji.scss',
  'sass/src/_entries.scss',
  'sass/src/_expander.scss',
  'sass/src/_filechooser.scss',
  'sass/src/_frame.scss',
  'sass/src/_headerbar.scss',
  'sass/src/_infobar.scss',
  'sass/src/_levelbar.scss',
  'sass/src/_links.scss',
  'sass/src/_lists.scss',
  'sass/src/_menu.scss',
  'sass/src/_misc.scss',
  'sass/src/_notebook.scss',
  'sass/src/_notifications.scss',
  'sass/src/_rounding.scss',
  'sass/src/_paned.scss',
  'sass/src/_pathbar.scss',
  'sass/src/_popover.scss',
  'sass/src/_printdialog.scss',
  'sass/src/_progressbar.scss',
  'sass/src/_scale.scss',
  'sass/src/_scrollbar.scss',
  'sass/src/_sidebar.scss',
  'sass/src/_spinbutton.scss',
  'sass/src/_spinner.scss',
  'sass/src/_switch.scss',
  'sass/src/_toolbar.scss',
  'sass/src/_tooltip.scss',
  'sass/src/_touchcopypaste.scss',
  'sass/src/_treeview.scss',
  'sass/src/_barryallen.scss',
]

gtk3_assets = [
  'assets/bullet-symbolic.svg',
  'assets/bullet-symbolic.symbolic.png',
  'assets/checkbox-active-selectionmode@2.png',
  'assets/checkbox-active-selectionmode.png',
  'assets/checkbox-backdrop-selectionmode@2.png',
  'assets/checkbox-backdrop-selectionmode.png',
  'assets/checkbox-checked-active-selectionmode@2.png',
  'assets/checkbox-checked-active-selectionmode.png',
  'assets/checkbox-checked-backdrop-selectionmode@2.png',
  'assets/checkbox-checked-backdrop-selectionmode.png',
  'assets/checkbox-checked-hover-selectionmode@2.png',
  'assets/checkbox-checked-hover-selectionmode.png',
  'assets/checkbox-checked-selectionmode@2.png',
  'assets/checkbox-checked-selectionmode.png',
  'assets/checkbox-hover-selectionmode@2.png',
  'assets/checkbox-hover-selectionmode.png',
  'assets/checkbox-selectionmode@2.png',
  'assets/checkbox-selectionmode.png',
  'assets/check-symbolic.svg',
  'assets/check-symbolic.symbolic.png',
  'assets/dash-symbolic.svg',
  'assets/dash-symbolic.symbolic.png',
  'assets/slider-horz-scale-has-marks-above@2.png',
  'assets/slider-horz-scale-has-marks-above-active@2.png',
  'assets/slider-horz-scale-has-marks-above-active.png',
  'assets/slider-horz-scale-has-marks-above-backdrop@2.png',
  'assets/slider-horz-scale-has-marks-above-backdrop-insensitive@2.png',
  'assets/slider-horz-scale-has-marks-above-backdrop-insensitive.png',
  'assets/slider-horz-scale-has-marks-above-backdrop.png',
  'assets/slider-horz-scale-has-marks-above-hover@2.png',
  'assets/slider-horz-scale-has-marks-above-hover.png',
  'assets/slider-horz-scale-has-marks-above-insensitive@2.png',
  'assets/slider-horz-scale-has-marks-above-insensitive.png',
  'assets/slider-horz-scale-has-marks-above.png',
  'assets/slider-horz-scale-has-marks-below@2.png',
  'assets/slider-horz-scale-has-marks-below-active@2.png',
  'assets/slider-horz-scale-has-marks-below-active.png',
  'assets/slider-horz-scale-has-marks-below-backdrop@2.png',
  'assets/slider-horz-scale-has-marks-below-backdrop-insensitive@2.png',
  'assets/slider-horz-scale-has-marks-below-backdrop-insensitive.png',
  'assets/slider-horz-scale-has-marks-below-backdrop.png',
  'assets/slider-horz-scale-has-marks-below-hover@2.png',
  'assets/slider-horz-scale-has-marks-below-hover.png',
  'assets/slider-horz-scale-has-marks-below-insensitive@2.png',
  'assets/slider-horz-scale-has-marks-below-insensitive.png',
  'assets/slider-horz-scale-has-marks-below.png',
  'assets/slider-vert-scale-has-marks-above@2.png',
  'assets/slider-vert-scale-has-marks-above-active@2.png',
  'assets/slider-vert-scale-has-marks-above-active.png',
  'assets/slider-vert-scale-has-marks-above-backdrop@2.png',
  'assets/slider-vert-scale-has-marks-above-backdrop-insensitive@2.png',
  'assets/slider-vert-scale-has-marks-above-backdrop-insensitive.png',
  'assets/slider-vert-scale-has-marks-above-backdrop.png',
  'assets/slider-vert-scale-has-marks-above-hover@2.png',
  'assets/slider-vert-scale-has-marks-above-hover.png',
  'assets/slider-vert-scale-has-marks-above-insensitive@2.png',
  'assets/slider-vert-scale-has-marks-above-insensitive.png',
  'assets/slider-vert-scale-has-marks-above.png',
  'assets/slider-vert-scale-has-marks-below@2.png',
  'assets/slider-vert-scale-has-marks-below-active@2.png',
  'assets/slider-vert-scale-has-marks-below-active.png',
  'assets/slider-vert-scale-has-marks-below-backdrop@2.png',
  'assets/slider-vert-scale-has-marks-below-backdrop-insensitive@2.png',
  'assets/slider-vert-scale-has-marks-below-backdrop-insensitive.png',
  'assets/slider-vert-scale-has-marks-below-backdrop.png',
  'assets/slider-vert-scale-has-marks-below-hover@2.png',
  'assets/slider-vert-scale-has-marks-below-hover.png',
  'assets/slider-vert-scale-has-marks-below-insensitive@2.png',
  'assets/slider-vert-scale-has-marks-below-insensitive.png',
  'assets/slider-vert-scale-has-marks-below.png',
  'assets/text-select-end@2.png',
  'assets/text-select-end-active@2.png',
  'assets/text-select-end-active.png',
  'assets/text-select-end-hover@2.png',
  'assets/text-select-end-hover.png',
  'assets/text-select-end.png',
  'assets/text-select-start@2.png',
  'assets/text-select-start-active@2.png',
  'assets/text-select-start-active.png',
  'assets/text-select-start-hover@2.png',
  'assets/text-select-start-hover.png',
  'assets/text-select-start.png',
  'assets/titlebutton-hover.png',
  'assets/titlebutton-hover@2.png',
  'assets/titlebutton-active.png',
  'assets/titlebutton-active@2.png',
  'assets/titlebutton-selection-mode-hover.png',
  'assets/titlebutton-selection-mode-hover@2.png',
  'assets/titlebutton-selection-mode-active.png',
  'assets/titlebutton-selection-mode-active@2.png',
  'assets/close-button.png',
  'assets/close-button@2.png',
  'assets/close-button-hover.png',
  'assets/close-button-hover@2.png',
  'assets/close-button-active.png',
  'assets/close-button-active@2.png',
  'assets/close-button-backdrop.png',
  'assets/close-button-backdrop@2.png',
  'assets/close-button-selection-mode.png',
  'assets/close-button-selection-mode@2.png'
]

# generate .css files
# and install to themes/THEMENAME/gtk-3.0
foreach f : gtk3_scss_sources
  custom_target('generate_' + f,
      input: f + '.scss',
      output: f + '.css',
      depend_files: files(gtk3_scss_dependencies),
      command: [sassc, '-a', '@INPUT@', '@OUTPUT@'],
      build_by_default: true,
      install: true,
      install_dir: gtk3_dir,
  )
endforeach

# Install asset files to themes/THEMENAME/gtk-3.0/assets
install_data(gtk3_assets, install_dir: gtk3_asset_dir)


