sassc = find_program('sassc')

gtk3_dir = join_paths(theme_dir, 'gtk-3.0')
gtk3_asset_dir = join_paths(gtk3_dir, 'assets')

# Dependencies of the files that need to be compiled
gtk3_scss_dependencies = [
  '../../Standard/gtk-3.0/sass/_starlabs.scss',
  '../../Standard/gtk-3.0/sass/_functions.scss',
  '../../Standard/gtk-3.0/sass/functions/_checkradio.scss',
  '../../Standard/gtk-3.0/sass/functions/_dialog_window.scss',
  '../../Standard/gtk-3.0/sass/functions/_font-size.scss',
  '../../Standard/gtk-3.0/sass/functions/_switch.scss',
  '../../Standard/gtk-3.0/sass/functions/_entries.scss',
  '../../Standard/gtk-3.0/sass/functions/_header.scss',
  '../../Standard/gtk-3.0/sass/functions/_undershoot.scss',
  '../../Standard/gtk-3.0/sass/functions/_clickable.scss',
  '../../Standard/gtk-3.0/sass/functions/_fill.scss',
  '../../Standard/gtk-3.0/sass/functions/_overshoot.scss',
  '../../Standard/gtk-3.0/sass/functions/_general.scss',
  '../../Standard/gtk-3.0/sass/_src.scss',
  '../../Standard/gtk-3.0/sass/src/_alpha.scss',
  '../../Standard/gtk-3.0/sass/src/_base.scss',
  '../../Standard/gtk-3.0/sass/src/_apps.scss',
  '../../Standard/gtk-3.0/sass/src/_button.scss',
  '../../Standard/gtk-3.0/sass/src/_calendar.scss',
  '../../Standard/gtk-3.0/sass/src/_checkradio.scss',
  '../../Standard/gtk-3.0/sass/src/_colorchooser.scss',
  '../../Standard/gtk-3.0/sass/src/_comboboxes.scss',
  '../../Standard/gtk-3.0/sass/src/_decoration.scss',
  '../../Standard/gtk-3.0/sass/src/_dialog.scss',
  '../../Standard/gtk-3.0/sass/src/_emoji.scss',
  '../../Standard/gtk-3.0/sass/src/_entries.scss',
  '../../Standard/gtk-3.0/sass/src/_expander.scss',
  '../../Standard/gtk-3.0/sass/src/_filechooser.scss',
  '../../Standard/gtk-3.0/sass/src/_frame.scss',
  '../../Standard/gtk-3.0/sass/src/_headerbar.scss',
  '../../Standard/gtk-3.0/sass/src/_infobar.scss',
  '../../Standard/gtk-3.0/sass/src/_levelbar.scss',
  '../../Standard/gtk-3.0/sass/src/_links.scss',
  '../../Standard/gtk-3.0/sass/src/_lists.scss',
  '../../Standard/gtk-3.0/sass/src/_menu.scss',
  '../../Standard/gtk-3.0/sass/src/_misc.scss',
  '../../Standard/gtk-3.0/sass/src/_notebook.scss',
  '../../Standard/gtk-3.0/sass/src/_notifications.scss',
  '../../Standard/gtk-3.0/sass/src/_rounding.scss',
  '../../Standard/gtk-3.0/sass/src/_paned.scss',
  '../../Standard/gtk-3.0/sass/src/_pathbar.scss',
  '../../Standard/gtk-3.0/sass/src/_popover.scss',
  '../../Standard/gtk-3.0/sass/src/_printdialog.scss',
  '../../Standard/gtk-3.0/sass/src/_progressbar.scss',
  '../../Standard/gtk-3.0/sass/src/_scale.scss',
  '../../Standard/gtk-3.0/sass/src/_scrollbar.scss',
  '../../Standard/gtk-3.0/sass/src/_sidebar.scss',
  '../../Standard/gtk-3.0/sass/src/_spinbutton.scss',
  '../../Standard/gtk-3.0/sass/src/_spinner.scss',
  '../../Standard/gtk-3.0/sass/src/_switch.scss',
  '../../Standard/gtk-3.0/sass/src/_toolbar.scss',
  '../../Standard/gtk-3.0/sass/src/_tooltip.scss',
  '../../Standard/gtk-3.0/sass/src/_touchcopypaste.scss',
  '../../Standard/gtk-3.0/sass/src/_treeview.scss',
  '../../Standard/gtk-3.0/sass/src/_barryallen.scss',
]

# generate .css files
# and install to themes/THEMENAME-Frost/gtk-3.0
custom_target('gtk3_dark',
    input: '../../Standard/gtk-3.0/gtk-dark.scss',
    output: 'gtk.css',
    depend_files: files(gtk3_scss_dependencies),
    command: [sassc, '-a', '@INPUT@', '@OUTPUT@'],
    build_by_default: true,
    install: true,
    install_dir: gtk3_dir,
)

# assets are just a symlink to the light themes as they are not modified
meson.add_install_script('sh', '-c', 'ln -sf ../../'+meson.project_name()+'/gtk-3.0/assets $MESON_INSTALL_DESTDIR_PREFIX/'+gtk3_asset_dir)
