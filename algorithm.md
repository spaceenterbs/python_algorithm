###### a
~~b~~
**c**

processPageOpenRequest ()
{
    if (current_count < MAX_COUNT)
    {
        sendResponse ();
        current_count++;
    }
    else
    {
        sendErrorMessage ();
    }
}

processPageCloseRequest ()
{
    current_count--;
}