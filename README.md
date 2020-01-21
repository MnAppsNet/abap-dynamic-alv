# ABAP Dynamic ALV
Create and display easily an ALV on ABAP

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
