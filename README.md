# dataset
 industry dataset include six major categories of entity types： equipment name, fault type, attribute information, operation action, normal state, and abnormal state. and seven relationship types: BEL, ATTR, PST, FAL, OPT, NS, and UNS.


A simple industrial example is shown in the following figure：
![image](https://github.com/user-attachments/assets/145e6c5b-7919-4472-b918-bc9975039193)

The Chinese data format is：
'{"tokens": ["自", "动", "加", "工", "，", "主", "轴", "抓", "刀", "再", "次", "报", "警", "，", "检", "查", "，", "交", "班", "。"], "entities": [{"type": "OPERATION", "start": 0, "end": 4}, {"type": "DEVICE", "start": 5, "end": 7}, {"type": "DEVICE", "start": 7, "end": 9}, {"type": "UNNORMAL", "start": 9, "end": 13}, {"type": "OPERATION", "start": 14, "end": 16}, {"type": "OPERATION", "start": 17, "end": 19}], "relations": [{"type": "PST", "head": 0, "tail": 4}, {"type": "OPT", "head": 4, "tail": 1}, {"type": "BEL", "head": 2, "tail": 1}, {"type": "UNS", "head": 3, "tail": 2}, {"type": "PST", "head": 4, "tail": 5}]}'

The English data format is：
' {"tokens": ["Automatic", "machining", "process", "encounters", "spindle", "tool", "grabbing", "Alarms", "again", "，", "requires", "immediate", "checking", "and", "shift", "changeover", "."], "entities": [{"type": "OPERATION", "start": 0, "end": 2}, {"type": "DEVICE", "start": 4, "end": 5}, {"type": "DEVICE", "start": 5, "end": 7}, {"type": "UNNORMAL", "start":7, "end": 9}, {"type": "OPERATION", "start": 13, "end": 14}, {"type": "OPERATION", "start": 15, "end": 17}], "relations": [{"type": "PST", "head": 0, "tail": 4}, {"type": "OPT", "head": 4, "tail": 1}, {"type": "BEL", "head": 2, "tail": 1}, {"type": "UNS", "head": 3, "tail": 2}, {"type": "PST", "head": 4, "tail": 5}]}'
