set(lib_TCLSCRIPTS
  Accordion.tcl
  CellPlot.tcl
  ColorEntry.tcl
  ComboBox.tcl
  Command.tcl
  Database.tcl
  Db.tcl
  Display.tcl
  Dm.tcl
  Drawable.tcl
  Ged.tcl
  GeometryIO.tcl
  Help.tcl
  Legend.tcl
  Mged.tcl
  ModelAxesControl.tcl
  QuadDisplay.tcl
  RtControl.tcl
  RtImage.tcl
  Splash.tcl
  Table.tcl
  TableView.tcl
  TkTable.tcl
  View.tcl
  ViewAxesControl.tcl
  cursor.tcl
  apply_mat.tcl
  gui_conversion.tcl
  pattern.tcl
  pattern_gui.tcl
  )
if (BRLCAD_ENABLE_TCL)
  BRLCAD_ADDDATA(lib_TCLSCRIPTS tclscripts/lib)
  pkgIndex_BUILD(tclscripts/lib)
  tclIndex_BUILD(tclscripts/lib)
endif (BRLCAD_ENABLE_TCL)

CMAKEFILES(
  CMakeLists.txt
  ${lib_TCLSCRIPTS}
  )

# Local Variables:
# tab-width: 8
# mode: cmake
# indent-tabs-mode: t
# End:
# ex: shiftwidth=2 tabstop=8
