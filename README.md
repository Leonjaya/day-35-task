# day-35-task
db.products.find({});
db.products.find({ price: { $gte: 400, $lte: 800 } });
db.products.find({ price: { $not: { $gte: 400, $lte: 600 } } });
db.products.find({ price: { $gt: 500 } }).limit(4);
db.products.find({}, { _id: 0, name: 1, material: 1 });
db.products.findOne({ id: 10 });
db.products.find({}, { _id: 0, name: 1, material: 1 });
db.products.find({ material: { $regex: /soft/i } });
db.products.find({ color: "indigo", price: 492.00 });
db.products.deleteMany({ price: 28 });
