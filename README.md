# ABAP Dynamic ALV
Create and display an ALV on ABAP easily

# How to use :
              > Use static method add_instraction to add a field on the output ALV
                It takes 2 mandatory field :
                  *im_table : the table refference that contains the field we want to add
                  *im_fieldname : the name of the field that we want to add to ALV
              > Use static method add_column_instraction to change ALV column properties
                It takes 2 mandatory field and 4 oprional :
                  *column_name        : The name of the column to make the changes
                  *column_text        : The header of the column
                  *column_text_medium : The medium size header of the column (optional, Default = column_text)
                  *column_text_short  : The short size header of the column  (optional, Default = column_text)
                  *column_length      : The length of the column             (optional, Default = Optimal)
                  *column_vissible    : The vissibility of the column        (optional, Default = Vissible)
              > Use static method create_alv to build the ALV and prepair for display
              > Use static method display_alv to display the ALV created (need to be created first)
              > Change global static object alv_table to make any further changes on the ALV output
                (need to be created first)
              > Use static method clear to discart all the instractions
              > Use static method dispose_alv to dispose the alv_table
              > Use static method row_count to get the number of rows of output table
              > Use static method get_field to get the value of a cell.
                It takes 3 parameters :
                 *im_row         : The row index that we want to get the field from
                 *im_column_name : The column name from which we get the value
                 *ch_content     : The value of the cell is returned here
              > Use static method get_row to get a row from table
                It takes 2 parameters :
                 *im_row         : The row index that we want to return
                 *ch_struct      : The row is returned here
              > Use static method get_selected_cell to get the value of selected cell
               It takes 1 parameter :
                 *ch_content     : The values of the cell is returned here
              > Use static method get_selected_row to get a selected row
               It takes 2 parameters :
                 *im_row_number : The row number from the rows selected (ex. 1st, 2nd ...) (optional, Default = 1 )
                 *ch_struct     : The row is returned here
