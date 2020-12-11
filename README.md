# autodesk_data

The data we use is the customer website visit records of seperate web activity of Autodesk.com. Each record is a dictionary specified the information of the website visit event. The meaning of the fields are:
- visit_id: Identifies a web session. Multiple rows of data can have the same visit_id. As suggested earlier this is expected, all rows with the same visit_id are part of the same session
- vistor_id: The known user’s ID of the visit
- customer_hit_date_time_pst: Time-stamp of the recorded event (web page view)
- product_line_id: product line id associated with page visit
- visit_number: given a constant visitor_id, this number identifies which session the current one is a part of, i.e., if cookies are saved then each time the user starts a new web session, this number increments by 1. If cookies are deleted then a new visitor_id is assigned and visit_number resets to 1 regardless of whether or not user_id is known.
- site_industry_group: Website user's industry group. Values are either ‘M&E’(marketing and entertainment) or ‘AEC’(achitecture, engineering & construction). Each unique known user is assigned an industry group.
- category: category of web page visited during this category.
