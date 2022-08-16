import folium
way1=[[16.780001,80.849998],[16.7850,80.8488],[16.6356,80.9716],[16.7107,81.0952],[16.8108,81.2637],[16.9479,81.4045],
      [16.9990,81.5061],[17.0350,81.5624],[16.9930,81.6668],[17.0005,81.8040],[17.2789,82.4013],[17.6868,83.2185],
      [17.9325,83.4268],[18.2949,83.8938],[18.40914429311417, 83.90322187347678],[18.60087363860685, 83.75803663010186]]
way2=[[16.780001,80.849998],[16.7180,81.1195],[16.8098,81.5267],[16.9847,81.7843],[17.046328668381637, 82.17115456308615],[17.279307388141994, 82.40039921731191],
      [17.358081520647865, 82.54333672174974],[17.689572103502417, 83.00291897428538],[17.68171551659318, 83.22481311670384],[18.111708629950332, 83.39512902489908],
      [18.40914429311417, 83.90322187347678],[18.60087363860685, 83.75803663010186]]
from branca.element import Figure
fig=Figure(width=550,height=350)
f1=folium.FeatureGroup("Vehicle 1")
f2=folium.FeatureGroup("Vehicle 2")
map=folium.Map(location=[16.780001,80.849998])
line_1=folium.vector_layers.PolyLine(way1,popup='<b>Path of Vehicle_1</b>',tooltip='Vehicle_1',color='blue',weight=10).add_to(f1)
line_2=folium.vector_layers.PolyLine(way2,popup='<b>Path of Vehicle_2</b>',tooltip='Vehicle_2',color='red',weight=10).add_to(f2)
f1.add_to(map)
f2.add_to(map)
folium.Marker(location=[16.780001,80.849998],popup='Starting point',tooltip='Nuzvidu').add_to(map)
folium.Marker(location=[18.60087363860685, 83.75803663010186],popup='Destination',tooltip='Palakonda').add_to(map)
folium.LayerControl().add_to(map)
map
