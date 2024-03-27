# asst_prof_salaries
Dataset of average assistant professor salaries across US public R1 institutions

## Data
* Average assistant professor salaries for year 2022: [AAUP Faculty Compensation Survey](https://data.aaup.org/ft-faculty-salaries/)
* County-level cost of living for family of 2 adults and 2 children for year 2023: [Economic Policy Institute Family Budget Map](https://www.epi.org/resources/budget/budget-map/). It should be noted that these estimates are enought to "attain a modest yet adequate standard of living", which translates to no savings and no mortgage (costs incorporate rent).
* List of public R1 institution in the US: [Wikipedia](https://en.wikipedia.org/wiki/List_of_research_universities_in_the_United_States)


Assignment of county (or unincorporated city) to universities was done by hand and based on the city where the main campus is located according to Wikipedia. For large cities spanning multiple counties, cost of living is the average between all of them.

Expected salary represents the value predicted by the linear regression.

The major caveat of this analysis is that the composition of assistant professors across universities can vary depending on the presence/absence/strength of different departments. For example, places with strong departments of engineering, business, economy, or other discipline with a high market value, would be biased upwards, while institutions without some/all of those departments would be biased downwards. Such large differences in composition could mean that the average salary is a poor predictor of the salary that would be offered to any incoming faculty.

## Table
A csv file with the data can be downloaded from this repository.

The visualization of it below was generated using https://csvtomd.com/#/

| University                                  | Average assistant professor salary | County/city                                      | Cost of living | Expected salary | Salary difference (actual - expected) | Relative difference (actual / expected) | Above average | Above 1:1 |
| ------------------------------------------- | ---------------------------------- | ------------------------------------------------ | -------------- | --------------- | ------------------------------------- | --------------------------------------- | ------------- | --------- |
| University of Texas at Dallas               | 125.6                              | Dallas County-Collin County                      | 103.6          | 93.4            | 32.2                                  | 134.5                                   | yes           | yes       |
| University of Texas at Austin               | 119.6                              | Travis County                                    | 108.6          | 95.3            | 24.3                                  | 125.5                                   | yes           | yes       |
| Georgia Institute of Technology             | 119.7                              | Fulton County                                    | 112.8          | 96.9            | 22.8                                  | 123.5                                   | yes           | yes       |
| University of California, Los Angeles       | 123.6                              | Los Angeles County                               | 130.1          | 103.5           | 20.1                                  | 119.4                                   | yes           | no        |
| Texas A&M University                        | 104.1                              | Brazos County                                    | 88.8           | 87.8            | 16.3                                  | 118.6                                   | yes           | yes       |
| University of California, Berkeley          | 129.5                              | Alameda County                                   | 155.9          | 113.4           | 16.1                                  | 114.2                                   | yes           | no        |
| University of California, San Diego         | 123.5                              | San Diego County                                 | 140.6          | 107.5           | 16.0                                  | 114.8                                   | yes           | no        |
| University of Maryland, College Park        | 111.2                              | Prince George's County                           | 110            | 95.9            | 15.3                                  | 116.0                                   | yes           | yes       |
| University of California, Davis             | 119.2                              | Yolo County                                      | 131.1          | 103.9           | 15.3                                  | 114.7                                   | yes           | no        |
| New Jersey Institute of Technology          | 109.2                              | Essex County                                     | 106.1          | 94.4            | 14.8                                  | 115.7                                   | yes           | yes       |
| University of Illinois Urbana-Champaign     | 107.1                              | Champaign County                                 | 102.4          | 93.0            | 14.1                                  | 115.2                                   | yes           | yes       |
| University of Houston                       | 103.5                              | Harris County                                    | 93.3           | 89.5            | 14.0                                  | 115.7                                   | yes           | yes       |
| University of Georgia                       | 102.3                              | Clarke County                                    | 91.3           | 88.7            | 13.6                                  | 115.3                                   | yes           | yes       |
| Indiana University Bloomington              | 104.7                              | Monroe County                                    | 99.5           | 91.8            | 12.9                                  | 114.0                                   | yes           | yes       |
| University of California, Riverside         | 111                                | Riverside County                                 | 117            | 98.5            | 12.5                                  | 112.7                                   | yes           | no        |
| University of Maryland, Baltimore County    | 103.5                              | Baltimore County                                 | 102.4          | 93.0            | 10.5                                  | 111.3                                   | yes           | yes       |
| Purdue University                           | 100.5                              | Tippecanoe County                                | 94.9           | 90.1            | 10.4                                  | 111.6                                   | yes           | yes       |
| Pennsylvania State University               | 106.9                              | Centre County                                    | 112.4          | 96.8            | 10.1                                  | 110.5                                   | yes           | no        |
| University of Michigan                      | 106.9                              | Washtenaw County                                 | 113.9          | 97.3            | 9.6                                   | 109.8                                   | yes           | no        |
| Clemson University                          | 97.4                               | Pickens County-Anderson County                   | 90             | 88.2            | 9.2                                   | 110.4                                   | yes           | yes       |
| Ohio State University                       | 100.5                              | Franklin County-Delaware County-Fairfield County | 99.7           | 91.9            | 8.6                                   | 109.3                                   | yes           | yes       |
| Virginia Tech                               | 100.9                              | Montgomery County                                | 100.9          | 92.4            | 8.5                                   | 109.2                                   | yes           | yes       |
| University of Florida                       | 97.2                               | Alachua County                                   | 94.1           | 89.8            | 7.4                                   | 108.3                                   | yes           | yes       |
| University of Delaware                      | 103.2                              | New Castle County                                | 111            | 96.2            | 7.0                                   | 107.2                                   | yes           | no        |
| University of Virginia                      | 104.4                              | Charlottesville city                             | 114.9          | 97.7            | 6.7                                   | 106.8                                   | yes           | no        |
| University of Texas at El Paso              | 91.1                               | El Paso County                                   | 80.7           | 84.7            | 6.4                                   | 107.6                                   | yes           | yes       |
| University of Wisconsin-Madison             | 105.8                              | Dane County                                      | 119.6          | 99.5            | 6.3                                   | 106.3                                   | yes           | no        |
| University of Arkansas                      | 93.6                               | Washington County                                | 87.7           | 87.3            | 6.3                                   | 107.2                                   | yes           | yes       |
| Mississippi State University                | 90.7                               | Oktibbeha County                                 | 80.3           | 84.5            | 6.2                                   | 107.3                                   | yes           | yes       |
| University of California, Santa Barbara     | 119.1                              | Santa Barbara County                             | 154.8          | 113.0           | 6.1                                   | 105.4                                   | yes           | no        |
| University of Illinois Chicago              | 101.6                              | Cook County-DuPage County                        | 112.4          | 96.8            | 4.8                                   | 105.0                                   | yes           | no        |
| Florida State University                    | 94                                 | Leon County                                      | 92.8           | 89.3            | 4.7                                   | 105.3                                   | yes           | yes       |
| University of Tennessee                     | 93.3                               | Knox County                                      | 91.1           | 88.6            | 4.7                                   | 105.3                                   | yes           | yes       |
| University of California, Irvine            | 114.3                              | Orange County                                    | 147            | 110.0           | 4.3                                   | 103.9                                   | yes           | no        |
| University of Kansas                        | 91.9                               | Douglas County                                   | 88.5           | 87.6            | 4.3                                   | 104.9                                   | yes           | yes       |
| University of Utah                          | 97.1                               | Salt Lake County                                 | 102.9          | 93.1            | 4.0                                   | 104.2                                   | yes           | no        |
| University of Kentucky                      | 93                                 | Fayette County                                   | 92.5           | 89.2            | 3.8                                   | 104.3                                   | yes           | yes       |
| University of Colorado Boulder              | 109                                | Boulder County                                   | 134.8          | 105.3           | 3.7                                   | 103.5                                   | yes           | no        |
| University of Colorado Denver               | 104.4                              | Denver County                                    | 125.2          | 101.7           | 2.7                                   | 102.7                                   | yes           | no        |
| Texas Tech University                       | 90.4                               | Lubbock County                                   | 88.6           | 87.7            | 2.7                                   | 103.1                                   | yes           | yes       |
| Florida International University            | 96.5                               | Miami-Dade County                                | 106            | 94.3            | 2.2                                   | 102.3                                   | yes           | no        |
| Temple University                           | 94.5                               | Philadelphia County                              | 100.9          | 92.4            | 2.1                                   | 102.3                                   | yes           | no        |
| University of Nebraska-Lincoln              | 95.4                               | Lancaster County                                 | 104.1          | 93.6            | 1.8                                   | 101.9                                   | yes           | no        |
| University of Oregon                        | 98.1                               | Lane County                                      | 113.5          | 97.2            | 0.9                                   | 100.9                                   | yes           | no        |
| University of South Carolina                | 90.2                               | Richland County                                  | 94.1           | 89.8            | 0.4                                   | 100.5                                   | yes           | no        |
| University of North Carolina at Chapel Hill | 95.3                               | Orange County-Durham County                      | 108.6          | 95.3            | 0.0                                   | 100.0                                   | yes           | no        |
| Auburn University                           | 91.4                               | Lee County                                       | 98.6           | 91.5            | -0.1                                  | 99.9                                    | no            | no        |
| University of Massachusetts Amherst         | 98.9                               | Hampshire County                                 | 118.4          | 99.1            | -0.2                                  | 99.8                                    | no            | no        |
| Louisiana State University                  | 91                                 | East Baton Rouge Parish                          | 97.9           | 91.2            | -0.2                                  | 99.7                                    | no            | no        |
| University of Missouri                      | 89.7                               | Boone County                                     | 94.5           | 89.9            | -0.2                                  | 99.7                                    | no            | no        |
| Michigan State University                   | 90.7                               | Ingham County-Clinton County                     | 98             | 91.3            | -0.6                                  | 99.4                                    | no            | no        |
| Iowa State University                       | 92.1                               | Story County                                     | 102.4          | 93.0            | -0.9                                  | 99.1                                    | no            | no        |
| University of Texas at San Antonio          | 89                                 | Bexar County-Comal County-Medina County          | 94.5           | 89.9            | -0.9                                  | 99.0                                    | no            | no        |
| University of Washington                    | 104.4                              | King County                                      | 135.1          | 105.4           | -1.0                                  | 99.0                                    | no            | no        |
| University of South Florida                 | 92.1                               | Hillsborough County                              | 102.9          | 93.1            | -1.0                                  | 98.9                                    | no            | no        |
| University of Iowa                          | 93.9                               | Johnson County                                   | 108            | 95.1            | -1.2                                  | 98.7                                    | no            | no        |
| University of Oklahoma                      | 89.5                               | Cleveland County                                 | 97             | 90.9            | -1.4                                  | 98.5                                    | no            | no        |
| Oregon State University                     | 97.9                               | Benton County                                    | 120            | 99.7            | -1.8                                  | 98.2                                    | no            | no        |
| Binghamton University                       | 91                                 | Broome County                                    | 102.2          | 92.9            | -1.9                                  | 98.0                                    | no            | no        |
| Old Dominion University                     | 87.9                               | Norfolk city                                     | 94.6           | 90.0            | -2.1                                  | 97.7                                    | no            | no        |
| University of Minnesota                     | 97.4                               | Hennepin County                                  | 119.9          | 99.6            | -2.2                                  | 97.8                                    | no            | no        |
| University of New Hampshire                 | 93.2                               | Strafford County                                 | 109            | 95.5            | -2.3                                  | 97.6                                    | no            | no        |
| University of Arizona                       | 86.8                               | Pima County                                      | 93             | 89.4            | -2.6                                  | 97.1                                    | no            | no        |
| Ohio University                             | 88.2                               | Athens County                                    | 97.9           | 91.2            | -3.0                                  | 96.7                                    | no            | no        |
| Arizona State University                    | 92.1                               | Maricopa County                                  | 108.2          | 95.2            | -3.1                                  | 96.8                                    | no            | no        |
| Colorado School of Mines                    | 99.2                               | Jefferson County                                 | 128            | 102.7           | -3.5                                  | 96.6                                    | no            | no        |
| University of Pittsburgh                    | 88.1                               | Allegheny County                                 | 99.6           | 91.9            | -3.8                                  | 95.9                                    | no            | no        |
| University of Connecticut                   | 97.8                               | Tolland County                                   | 125.1          | 101.6           | -3.8                                  | 96.2                                    | no            | no        |
| University of Hawaii at Manoa               | 98.7                               | Honolulu County                                  | 128.3          | 102.8           | -4.1                                  | 96.0                                    | no            | no        |
| University of California, Santa Cruz        | 115.8                              | Santa Cruz County                                | 174.1          | 120.3           | -4.5                                  | 96.2                                    | no            | no        |
| University of Alabama at Birmingham         | 87.3                               | Jefferson County                                 | 100.7          | 92.3            | -5.0                                  | 94.6                                    | no            | no        |
| Oklahoma State University-Stillwater        | 83.1                               | Payne County                                     | 89.9           | 88.2            | -5.1                                  | 94.2                                    | no            | no        |
| Wayne State University                      | 84.2                               | Wayne County                                     | 93.1           | 89.4            | -5.2                                  | 94.2                                    | no            | no        |
| Kansas State University                     | 81.7                               | Riley County                                     | 90.1           | 88.3            | -6.6                                  | 92.6                                    | no            | no        |
| University of Central Florida               | 86.8                               | Orange County                                    | 103.5          | 93.4            | -6.6                                  | 93.0                                    | no            | no        |
| University of Alabama in Huntsville         | 84.8                               | Madison County                                   | 98.6           | 91.5            | -6.7                                  | 92.7                                    | no            | no        |
| University of Alabama                       | 82.9                               | Tuscaloosa County                                | 94             | 89.7            | -6.8                                  | 92.4                                    | no            | no        |
| Washington State University                 | 81.1                               | Whitman County                                   | 91.6           | 88.8            | -7.7                                  | 91.3                                    | no            | no        |
| University of New Mexico                    | 80.6                               | Bernalillo County                                | 92             | 89.0            | -8.4                                  | 90.6                                    | no            | no        |
| North Carolina State University             | 87.2                               | Wake County                                      | 109.8          | 95.8            | -8.6                                  | 91.0                                    | no            | no        |
| University of Memphis                       | 77.9                               | Shelby County                                    | 86             | 86.7            | -8.8                                  | 89.9                                    | no            | no        |
| Virginia Commonwealth University            | 82.7                               | Richmond city                                    | 99.7           | 91.9            | -9.2                                  | 90.0                                    | no            | no        |
| Rutgers University-New Brunswick            | 93.4                               | Middlesex County                                 | 127.8          | 102.7           | -9.3                                  | 91.0                                    | no            | no        |
| North Dakota State University               | 75.9                               | Cass County                                      | 82.1           | 85.2            | -9.3                                  | 89.1                                    | no            | no        |
| University of Cincinnati                    | 80.9                               | Hamilton County                                  | 95.3           | 90.2            | -9.3                                  | 89.6                                    | no            | no        |
| University of Louisville                    | 79.5                               | Jefferson County                                 | 92.5           | 89.2            | -9.7                                  | 89.1                                    | no            | no        |
| Utah State University                       | 79.6                               | Cache County                                     | 95.4           | 90.3            | -10.7                                 | 88.2                                    | no            | no        |
| University at Albany, SUNY                  | 88.5                               | Albany County                                    | 118.8          | 99.2            | -10.7                                 | 89.2                                    | no            | no        |
| University at Buffalo                       | 84.2                               | Erie County                                      | 107.7          | 95.0            | -10.8                                 | 88.7                                    | no            | no        |
| George Mason University                     | 97.6                               | Fairfax County                                   | 146.3          | 109.7           | -12.1                                 | 89.0                                    | no            | no        |
| Colorado State University                   | 87.3                               | Larimer County                                   | 124.1          | 101.2           | -13.9                                 | 86.2                                    | no            | no        |
| University of Wisconsin-Milwaukee           | 81.6                               | Milwaukee County                                 | 109.4          | 95.6            | -14.0                                 | 85.3                                    | no            | no        |
| Kent State University                       | 76.1                               | Portage County                                   | 97.7           | 91.2            | -15.1                                 | 83.5                                    | no            | no        |
| Stony Brook University                      | 100                                | Suffolk County                                   | 162.9          | 116.1           | -16.1                                 | 86.2                                    | no            | no        |
| Montana State University                    | 77.6                               | Gallatin County                                  | 104.3          | 93.7            | -16.1                                 | 82.8                                    | no            | no        |
| Graduate Center, CUNY                       | 98                                 | New York County                                  | 160.2          | 115.0           | -17.0                                 | 85.2                                    | no            | no        |
| University of Southern Mississippi          | 67.9                               | Forrest County                                   | 83.8           | 85.9            | -18.0                                 | 79.1                                    | no            | no        |
| University of Nevada, Reno                  | 77.8                               | Washoe County                                    | 112.3          | 96.7            | -18.9                                 | 80.4                                    | no            | no        |
| University of Maine                         | 71.7                               | Penobscot County                                 | 97.9           | 91.2            | -19.5                                 | 78.6                                    | no            | no        |
| University of Nevada, Las Vegas             | 74                                 | Clark County                                     | 104.8          | 93.9            | -19.9                                 | 78.8                                    | no            | no        |
| Georgia State University                    | 75.8                               | Fulton County                                    | 112.8          | 96.9            | -21.1                                 | 78.2                                    | no            | no        |
| University of Montana                       | 69.2                               | Missoula County                                  | 102.4          | 93.0            | -23.8                                 | 74.4                                    | no            | no        |
|                                             |

## Plot
Plotting was done in R using *ggplot* and *ggrepel*. Labels were added to 1/5th of dots, selected at random.

![plot](https://github.com/mongiardino/asst_prof_salaries/blob/main/salary_plot.jpg)
**Fig. 1:** Average assistant professor salary against county-level cost of living for a family of four. All values are annual and expressed in thousands of dollars. Both a 1:1 line and a linear regression (with confidence interval) are plotted and used to classify universities into three categories.


