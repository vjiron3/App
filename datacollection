import React, { useState } from "react";
import { Button, Input, Textarea } from "@/components/ui";

const DataCollectionForm = () => {
  const [formData, setFormData] = useState({
    timestamp: new Date().toISOString(),
    email: "",
    customer: "",
    dieNumber: "",
    materialPartNumber: "",
    lotNumber: "",
    colorPartNumber: "",
    color: "",
    colorLotNumber: "",
    regrind: "",
    stageOfProduction: "",
    machine: "",
    machineAmps: "",
    screwSpeed: "",
    oilTemperature: "",
    doorTemperature: "",
    flangeTemperature: "",
    backPressure: "",
    feetPerHour: "",
    colorFeedRate: "",
    feederRpm: "",
    barrelTempZone1: "",
    barrelTempZone2: "",
    barrelTempZone3: "",
    barrelTempZone4: "",
    barrelTempZone5: "",
    dieSettingsTop: "",
    dieSettingsBottom: "",
    dieSettingsNorth: "",
    dieSettingsSouth: "",
    operatorInitials: "",
    partWeightPerFoot: "",
    scrapPounds: "",
    comments: ""
  });

  const handleChange = (e) => {
    setFormData({ ...formData, [e.target.name]: e.target.value });
  };

  const handleSubmit = async (e) => {
    e.preventDefault();
    console.log("Submitting Data:", formData);
    // TODO: Send data to Google Sheets or database
  };

  return (
    <div className="p-4 max-w-md mx-auto">
      <h1 className="text-xl font-bold mb-4">Data Collection</h1>
      <form onSubmit={handleSubmit}>
        <Input name="email" placeholder="Email Address" onChange={handleChange} required />
        <Input name="customer" placeholder="Customer" onChange={handleChange} required />
        <Input name="dieNumber" placeholder="Die Number" onChange={handleChange} />
        <Input name="materialPartNumber" placeholder="Material Part Number" onChange={handleChange} />
        <Input name="lotNumber" placeholder="Lot Number" onChange={handleChange} />
        <Input name="colorPartNumber" placeholder="Color Part Number" onChange={handleChange} />
        <Input name="color" placeholder="Color" onChange={handleChange} />
        <Input name="colorLotNumber" placeholder="Color Lot Number" onChange={handleChange} />
        <Input name="regrind" placeholder="Regrind" onChange={handleChange} />
        <Input name="stageOfProduction" placeholder="Stage of Production" onChange={handleChange} />
        <Input name="machine" placeholder="Machine" onChange={handleChange} />
        <Input name="machineAmps" placeholder="Machine AMPS" onChange={handleChange} type="number" />
        <Input name="screwSpeed" placeholder="Screw Speed / Motor RPM" onChange={handleChange} type="number" />
        <Input name="oilTemperature" placeholder="Oil Temperature" onChange={handleChange} type="number" />
        <Input name="doorTemperature" placeholder="Door Temperature" onChange={handleChange} type="number" />
        <Input name="flangeTemperature" placeholder="Flange Temperature" onChange={handleChange} type="number" />
        <Input name="backPressure" placeholder="Machine Back Pressure" onChange={handleChange} type="number" />
        <Input name="feetPerHour" placeholder="Feet Per Hour" onChange={handleChange} type="number" />
        <Input name="colorFeedRate" placeholder="Color Feed Rate" onChange={handleChange} type="number" />
        <Input name="feederRpm" placeholder="Feeder RPM" onChange={handleChange} type="number" />
        <Input name="barrelTempZone1" placeholder="Barrel Temperature Zone 1" onChange={handleChange} type="number" />
        <Input name="barrelTempZone2" placeholder="Barrel Temperature Zone 2" onChange={handleChange} type="number" />
        <Input name="barrelTempZone3" placeholder="Barrel Temperature Zone 3" onChange={handleChange} type="number" />
        <Input name="barrelTempZone4" placeholder="Barrel Temperature Zone 4" onChange={handleChange} type="number" />
        <Input name="barrelTempZone5" placeholder="Barrel Temperature Zone 5" onChange={handleChange} type="number" />
        <Input name="dieSettingsTop" placeholder="Die Settings Top" onChange={handleChange} />
        <Input name="dieSettingsBottom" placeholder="Die Settings Bottom" onChange={handleChange} />
        <Input name="dieSettingsNorth" placeholder="Die Settings North" onChange={handleChange} />
        <Input name="dieSettingsSouth" placeholder="Die Settings South" onChange={handleChange} />
        <Input name="operatorInitials" placeholder="Operator Initials" onChange={handleChange} required />
        <Input name="partWeightPerFoot" placeholder="Current Part Weight Per Foot" onChange={handleChange} type="number" />
        <Input name="scrapPounds" placeholder="Scrap Pounds per Shift" onChange={handleChange} type="number" />
        <Textarea name="comments" placeholder="Comments or Notes" onChange={handleChange} />
        <Button type="submit" className="mt-4 w-full">Submit</Button>
      </form>
    </div>
  );
};

export default DataCollectionForm;
