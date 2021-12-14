def func(df,groupby_col,change_col):
    for o,(key,sub_df) in enumerate(df.groupby(groupby_col)):
        
        
        ## get the new text
        ori_text=str(key)
        new_text_list=[ori_text+"_"+str(e) for e in range(len(sub_df))]
        
        
        ## change
        sub_df[change_col]=new_text_list
        
        
        ##append
        if o==0:
            final_df=sub_df
        else:
            final_df=final_df.append(sub_df)
    return(final_df)
