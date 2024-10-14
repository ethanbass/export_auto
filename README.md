Macro and instructions to export raw data from chemstation as CSV files.

# Instructions
1. Copy export_auto.MAC to Chem32/CORE.
2. Open chemstation and type ‘macro export_auto.MAC’ into the command line to load the macro.
3. Load method ‘EXPORTCSV.M’ (or create your own method that loads the 'export_auto.MAC' macro).
4. Open the data analysis view and open the sequence table for the sequence that you want to export.
5. Use the filldown wizard to ‘filldown’ all lines with ‘EXPORTCSV2’ as the method.
6. Reprocess the sequence to export your data as CSVs.

The CSVs will be exported in a folder called ‘EXPORT3D’ inside the folder for the sequence that you’ve reprocessed. (Warning: There is a bug that occasionally causes the macro to repeatedly export the first chromatogram in a sequence under different filenames. It is advisable to open the EXPORT3D folder and check that your converted chromatograms do not have identical file sizes. The bug can be usually be fixed by repeating the process outlined above from step 2).
