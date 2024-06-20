# ucus_yonetim_sistemi
Patika OOP Ödevi

Havayolu (Airline)

airlineID: int
name: String
planes: List[Plane]
pilots: List[Pilot]
Uçak (Plane)

planeID: int
type: String
status: PlaneStatus (enum: {Working, UnderMaintenance})
airline: Airline
Uçuş (Flight)

flightID: int
departureAirport: Airport
arrivalAirport: Airport
departureTime: DateTime
arrivalTime: DateTime
pilot: Pilot
coPilot: Pilot
plane: Plane
Havaalanı (Airport)

airportID: int
name: String
location: String
Pilot

pilotID: int
name: String
experienceLevel: int
airline: Airline
canFly: List[PlaneType]
Uçak Tipi (PlaneType)

typeID: int
typeName: String
requiredPilots: int
planes: List[Plane]
Uçak Durumu (PlaneStatus)

statusID: int
statusName: String (enum: {Working, UnderMaintenance})
