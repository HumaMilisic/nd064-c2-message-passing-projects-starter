frontend 

http://localhost:30001/api/persons

http://localhost:30001/api/persons/${personId}/connection?start_date=2020-01-01&end_date=2020-12-30&distance=5


api rest

@api.route("/locations")
@api.route("/locations/<location_id>")

@api.route("/persons")

@api.route("/persons/<person_id>")
@api.param("person_id", "Unique ID for a given Person", _in="query")


@api.route("/persons/<person_id>/connection")
@api.param("start_date", "Lower bound of date range", _in="query")
@api.param("end_date", "Upper bound of date range", _in="query")
@api.param("distance", "Proximity to a given user in meters", _in="query")


database