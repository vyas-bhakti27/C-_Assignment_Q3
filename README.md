#include <bits/stdc++.h>
using namespace std;
int main()
{
    ifstream fin;
    // string str;
    fin.open("file.txt");
    int count = 0;
    char str[30];
    int i = 0;

    if (!fin)
    {
        cout << "file did not open" << endl;
    }
    else
    {

        while (!fin.eof())
        {
            fin >> str;
            if (str[0] == 'e' || str[0] == 'E')
            {
                count++;
            }
        }
    }

    cout << "total words starting with e = " << count << endl;
    fin.close();
}

