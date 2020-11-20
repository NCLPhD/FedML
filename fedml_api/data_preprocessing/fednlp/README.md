## Performance
| dataset&partition | center | worker | center(tokenized) | worker(tokenized) | center size | worker size | number of clients | center storage cost(tokenized) | worker storage cost(tokenized) | center storage cost | worker storage cost |
| ------------ | ------------- | ------------- | ------------- | ------------- | ------------- | ------------- | ------------- | ------------- | ------------- | ------------- | ------------- |
| Cornell Movie & Uniform | 3.5s  | 2.9s | 87.9s | 7.8s | 221616 | 2217 | 100 | 4.5GB | 18MB | 72MB | 2MB |
| Cornell Movie & Nature | 2.8s | 2.0s | 84.4s | 2.0s | 221616 | - | 617 | 4.5GB | - | - | - |
| WMT & Uniform | 0.75s | 0.73s | 76.7s | 1.7s | 218384 | 2184 | 100 | - | - | - | - |
| wikigold & Uniform | 0.08s | 0.04s | - | - | 1841 | 19 | 100 | - | - | - | - |
| W_NUT 2017 & Uniform | 0.3s | 0.2s | - | - | 8444 | 85 | 100 | - | - | - | - |
| W_NUT 2017 & Nature | 0.25s | 0.17s | - | - | 8444 | - | 370 | - | - | - | - |
| CNN DailyMail & Uniform | 17.7s | 9.2s | 322.6s | 142.8s | 287227 | 2873 | 100 | - | - | - | - |

Cornell Nature Data Distribution
Counter({289: 1192, 295: 1161, 299: 1095, 82: 974, 105: 961, 428: 922, 238: 920, 513: 909, 243: 855, 90: 840, 522: 834, 77: 820, 537: 815, 342: 806, 435: 793, 380: 791, 246: 786, 16: 784, 149: 776, 72: 771, 100: 769, 528: 764, 532: 761, 234: 755, 467: 751, 139: 748, 588: 746, 368: 744, 35: 737, 127: 734, 175: 733, 333: 732, 423: 701, 103: 696, 244: 694, 208: 693, 293: 690, 373: 684, 150: 683, 152: 683, 296: 675, 292: 670, 475: 663, 88: 651, 163: 650, 78: 643, 38: 640, 202: 640, 229: 639, 569: 634, 312: 632, 595: 632, 55: 623, 178: 619, 230: 618, 487: 617, 42: 614, 269: 610, 519: 610, 106: 604, 118: 596, 348: 591, 217: 581, 225: 578, 140: 577, 347: 575, 593: 575, 119: 573, 355: 570, 266: 567, 564: 567, 62: 566, 291: 564, 589: 564, 598: 559, 104: 555, 329: 552, 141: 546, 278: 546, 381: 545, 518: 545, 94: 542, 586: 542, 70: 540, 575: 540, 231: 539, 427: 539, 503: 538, 565: 535, 36: 530, 431: 530, 533: 530, 469: 529, 594: 528, 27: 527, 204: 527, 285: 527, 369: 527, 444: 526, 539: 526, 336: 524, 276: 519, 516: 519, 20: 518, 275: 518, 112: 516, 370: 516, 10: 512, 314: 510, 251: 509, 334: 509, 102: 508, 109: 508, 491: 505, 507: 505, 376: 501, 332: 499, 570: 499, 124: 498, 267: 496, 89: 495, 324: 495, 2: 494, 239: 494, 464: 494, 216: 493, 552: 492, 601: 492, 298: 489, 451: 489, 463: 489, 465: 489, 126: 486, 605: 486, 283: 482, 341: 481, 499: 480, 161: 479, 462: 479, 330: 478, 120: 474, 479: 474, 512: 474, 450: 473, 151: 472, 327: 472, 101: 470, 162: 469, 250: 469, 0: 468, 287: 466, 19: 465, 181: 465, 482: 463, 220: 461, 167: 457, 6: 455, 536: 455, 550: 454, 29: 453, 199: 453, 322: 453, 17: 452, 402: 452, 371: 450, 363: 449, 194: 448, 374: 448, 201: 447, 144: 446, 224: 446, 403: 445, 168: 444, 309: 444, 560: 442, 169: 439, 93: 438, 235: 438, 302: 438, 416: 437, 511: 435, 83: 434, 48: 432, 240: 432, 247: 432, 397: 431, 455: 431, 92: 429, 131: 429, 214: 427, 25: 426, 545: 425, 591: 424, 79: 423, 405: 423, 495: 423, 573: 422, 527: 421, 84: 418, 59: 417, 304: 417, 344: 416, 279: 414, 615: 414, 45: 413, 205: 413, 404: 412, 453: 412, 418: 410, 249: 409, 281: 409, 111: 408, 207: 407, 18: 406, 494: 406, 129: 405, 193: 404, 308: 404, 320: 404, 236: 403, 424: 403, 128: 400, 306: 398, 496: 398, 610: 398, 4: 397, 273: 396, 198: 393, 57: 389, 203: 389, 471: 389, 54: 387, 408: 387, 558: 387, 501: 386, 257: 384, 44: 383, 303: 383, 335: 382, 568: 380, 337: 379, 200: 378, 288: 378, 326: 378, 21: 376, 32: 376, 50: 376, 71: 376, 445: 376, 525: 376, 390: 375, 358: 373, 190: 372, 389: 372, 66: 371, 68: 371, 301: 371, 446: 370, 561: 369, 133: 368, 165: 367, 22: 366, 87: 366, 132: 366, 415: 365, 46: 363, 508: 363, 154: 362, 294: 361, 576: 360, 23: 359, 174: 359, 353: 359, 256: 358, 367: 357, 166: 356, 581: 356, 599: 356, 170: 355, 117: 353, 316: 353, 411: 353, 352: 352, 34: 349, 318: 349, 113: 348, 123: 348, 449: 348, 419: 347, 265: 345, 53: 344, 606: 343, 130: 342, 480: 341, 37: 340, 171: 339, 252: 338, 436: 338, 556: 337, 75: 336, 284: 336, 530: 336, 65: 335, 433: 335, 505: 335, 24: 334, 74: 334, 197: 334, 228: 333, 541: 332, 164: 331, 442: 331, 502: 331, 544: 331, 300: 329, 375: 329, 407: 329, 443: 329, 506: 329, 585: 329, 215: 328, 429: 327, 458: 327, 221: 326, 188: 325, 399: 325, 437: 324, 282: 323, 546: 323, 553: 323, 172: 322, 195: 322, 498: 322, 160: 319, 540: 319, 69: 318, 122: 318, 313: 318, 514: 317, 554: 317, 577: 316, 159: 314, 534: 314, 391: 313, 603: 313, 147: 312, 517: 311, 192: 310, 223: 310, 426: 310, 434: 310, 136: 309, 395: 309, 286: 308, 145: 307, 233: 307, 454: 307, 548: 307, 613: 307, 452: 305, 388: 304, 457: 304, 441: 301, 41: 300, 107: 300, 219: 300, 366: 300, 582: 299, 212: 298, 258: 293, 481: 293, 189: 291, 386: 291, 472: 291, 121: 290, 211: 290, 39: 289, 98: 289, 180: 289, 377: 287, 422: 284, 597: 284, 356: 283, 485: 283, 5: 282, 413: 282, 473: 282, 524: 281, 58: 280, 345: 280, 387: 280, 185: 279, 125: 278, 143: 278, 30: 277, 108: 277, 196: 277, 331: 277, 383: 277, 157: 274, 248: 273, 187: 272, 280: 272, 43: 271, 31: 270, 365: 270, 448: 270, 592: 269, 76: 263, 488: 262, 555: 261, 574: 261, 609: 260, 28: 258, 33: 258, 146: 258, 346: 258, 578: 258, 587: 257, 520: 256, 526: 256, 310: 255, 612: 254, 476: 253, 493: 252, 52: 251, 60: 251, 186: 251, 579: 251, 583: 251, 63: 250, 394: 250, 268: 249, 425: 249, 115: 248, 461: 246, 492: 246, 261: 245, 343: 245, 378: 245, 509: 244, 209: 243, 142: 240, 563: 240, 155: 239, 290: 239, 11: 238, 241: 238, 379: 238, 156: 237, 468: 235, 432: 233, 49: 232, 97: 232, 260: 232, 572: 231, 523: 230, 417: 229, 596: 229, 400: 228, 497: 227, 47: 226, 61: 226, 99: 226, 245: 226, 15: 225, 542: 224, 222: 223, 420: 223, 584: 223, 396: 221, 51: 218, 173: 218, 213: 218, 254: 217, 372: 217, 14: 214, 262: 213, 110: 211, 253: 211, 607: 211, 153: 210, 183: 210, 232: 210, 137: 209, 392: 209, 12: 208, 191: 208, 67: 205, 410: 205, 177: 204, 321: 204, 421: 204, 551: 204, 385: 203, 611: 203, 274: 201, 305: 201, 357: 201, 73: 200, 3: 199, 91: 199, 227: 199, 477: 199, 40: 198, 158: 198, 430: 198, 531: 197, 566: 197, 86: 195, 500: 195, 529: 195, 401: 193, 80: 192, 398: 192, 351: 191, 590: 189, 116: 187, 218: 185, 264: 185, 409: 182, 134: 181, 323: 181, 1: 180, 438: 180, 393: 178, 237: 177, 447: 177, 114: 176, 439: 176, 608: 176, 182: 175, 259: 175, 272: 175, 538: 175, 557: 174, 340: 173, 319: 172, 148: 171, 489: 170, 339: 166, 179: 165, 242: 165, 255: 165, 263: 165, 311: 164, 547: 163, 571: 162, 549: 160, 13: 158, 504: 158, 460: 157, 349: 156, 412: 156, 604: 154, 543: 153, 210: 152, 325: 152, 440: 151, 474: 151, 317: 149, 362: 149, 466: 149, 382: 144, 315: 142, 384: 141, 64: 139, 328: 138, 9: 136, 354: 133, 271: 132, 490: 132, 364: 128, 226: 125, 359: 125, 81: 124, 184: 122, 360: 122, 361: 122, 535: 122, 8: 121, 96: 119, 562: 119, 515: 116, 614: 116, 297: 113, 56: 110, 176: 108, 307: 105, 600: 105, 7: 103, 135: 103, 510: 103, 138: 97, 277: 95, 567: 95, 26: 91, 414: 90, 559: 87, 483: 84, 350: 81, 470: 80, 85: 77, 580: 70, 95: 68, 478: 67, 616: 50, 459: 49, 206: 45, 338: 34, 486: 34, 484: 24, 456: 20, 406: 12, 521: 10, 270: 8, 602: 5})

W_NUT Nature Data Distribution
Counter({359: 181, 28: 159, 291: 159, 2: 113, 44: 111, 138: 98, 325: 93, 222: 88, 227: 84, 137: 77, 3: 72, 329: 71, 263: 69, 243: 67, 63: 65, 120: 65, 356: 65, 217: 64, 265: 63, 368: 56, 261: 54, 5: 52, 45: 51, 27: 49, 155: 46, 49: 45, 68: 45, 110: 44, 313: 44, 157: 43, 205: 43, 43: 42, 85: 42, 103: 42, 139: 42, 150: 42, 279: 42, 4: 41, 77: 41, 23: 40, 331: 40, 136: 39, 166: 39, 267: 39, 322: 39, 39: 38, 124: 38, 303: 38, 109: 37, 115: 37, 154: 37, 201: 37, 249: 37, 269: 37, 360: 37, 310: 36, 343: 36, 53: 35, 122: 35, 213: 35, 237: 35, 42: 34, 86: 33, 146: 33, 170: 33, 174: 33, 183: 33, 212: 33, 25: 32, 48: 32, 58: 32, 207: 32, 239: 32, 260: 32, 66: 31, 70: 31, 95: 31, 148: 31, 230: 31, 266: 31, 311: 31, 327: 31, 344: 31, 362: 31, 0: 30, 47: 30, 91: 30, 132: 30, 186: 30, 290: 30, 361: 30, 15: 29, 67: 29, 81: 29, 89: 29, 101: 29, 188: 29, 204: 29, 215: 29, 248: 29, 307: 29, 22: 28, 24: 28, 29: 28, 52: 28, 56: 28, 147: 28, 156: 28, 177: 28, 187: 28, 229: 28, 317: 28, 326: 28, 335: 28, 352: 28, 36: 27, 93: 27, 130: 27, 171: 27, 225: 27, 278: 27, 346: 27, 353: 27, 17: 26, 40: 26, 71: 26, 98: 26, 100: 26, 153: 26, 270: 26, 345: 26, 16: 25, 73: 25, 104: 25, 144: 25, 241: 25, 354: 25, 62: 24, 90: 24, 99: 24, 134: 24, 184: 24, 282: 24, 323: 24, 342: 24, 363: 24, 366: 24, 7: 23, 59: 23, 76: 23, 82: 23, 92: 23, 116: 23, 123: 23, 140: 23, 141: 23, 193: 23, 211: 23, 245: 23, 247: 23, 254: 23, 256: 23, 268: 23, 297: 23, 355: 23, 10: 22, 51: 22, 55: 22, 69: 22, 246: 22, 259: 22, 284: 22, 295: 22, 298: 22, 33: 21, 74: 21, 78: 21, 87: 21, 105: 21, 142: 21, 145: 21, 172: 21, 206: 21, 226: 21, 274: 21, 277: 21, 293: 21, 338: 21, 348: 21, 20: 20, 75: 20, 114: 20, 117: 20, 151: 20, 152: 20, 161: 20, 190: 20, 209: 20, 223: 20, 308: 20, 312: 20, 324: 20, 351: 20, 364: 20, 162: 19, 176: 19, 218: 19, 242: 19, 258: 19, 283: 19, 305: 19, 315: 19, 341: 19, 9: 18, 18: 18, 32: 18, 54: 18, 61: 18, 79: 18, 129: 18, 164: 18, 216: 18, 328: 18, 357: 18, 1: 17, 19: 17, 26: 17, 30: 17, 111: 17, 128: 17, 160: 17, 169: 17, 234: 17, 281: 17, 304: 17, 12: 16, 127: 16, 133: 16, 159: 16, 173: 16, 191: 16, 203: 16, 250: 16, 41: 15, 125: 15, 208: 15, 210: 15, 238: 15, 264: 15, 287: 15, 300: 15, 11: 14, 13: 14, 88: 14, 135: 14, 158: 14, 195: 14, 198: 14, 199: 14, 235: 14, 286: 14, 289: 14, 302: 14, 336: 14, 350: 14, 8: 13, 21: 13, 97: 13, 149: 13, 167: 13, 179: 13, 185: 13, 224: 13, 276: 13, 334: 13, 358: 13, 365: 13, 37: 12, 84: 12, 94: 12, 119: 12, 121: 12, 181: 12, 189: 12, 251: 12, 252: 12, 257: 12, 271: 12, 306: 12, 319: 12, 321: 12, 340: 12, 31: 11, 34: 11, 64: 11, 72: 11, 106: 11, 178: 11, 196: 11, 214: 11, 232: 11, 244: 11, 273: 11, 288: 11, 296: 11, 299: 11, 314: 11, 347: 11, 349: 11, 369: 11, 38: 10, 57: 10, 60: 10, 65: 10, 112: 10, 163: 10, 165: 10, 175: 10, 182: 10, 197: 10, 220: 10, 221: 10, 240: 10, 309: 10, 320: 10, 333: 10, 337: 10, 367: 10, 14: 9, 46: 9, 50: 9, 83: 9, 107: 9, 126: 9, 236: 9, 253: 9, 6: 8, 35: 8, 96: 8, 108: 8, 113: 8, 131: 8, 143: 8, 192: 8, 228: 8, 231: 8, 233: 8, 262: 8, 272: 8, 285: 8, 292: 8, 301: 8, 339: 8, 102: 7, 180: 7, 194: 7, 219: 7, 280: 7, 294: 7, 330: 7, 332: 7, 168: 6, 200: 6, 202: 6, 275: 6, 318: 6, 118: 5, 316: 5, 80: 4, 255: 4})

SemEval2010Task8 Natural Data Distribution:
Counter({1: 1410, 5: 844, 4: 659, 9: 612, 10: 568, 7: 490, 0: 471, 12: 470, 2: 407, 8: 394, 6: 374, 11: 344, 14: 323, 16: 166, 15: 148, 13: 144, 17: 97, 3: 78, 18: 1})

Sentiment140 Natural Data Distribution:
Counter({34: 111676, 29: 110290, 37: 109781, 27: 103673, 35: 96350, 28: 94588, 26: 73827, 38: 67980, 30: 64192, 33: 58757, 42: 45364, 39: 44012, 41: 43136, 40: 43004, 31: 41588, 17: 40154, 20: 39074, 18: 36469, 9: 35333, 4: 27469, 8: 27434, 12: 26029, 3: 21754, 47: 19694, 5: 18460, 15: 17460, 1: 17311, 45: 17002, 43: 16360, 25: 15903, 10: 15481, 44: 12009, 11: 11739, 23: 10778, 16: 9146, 6: 8587, 36: 8272, 32: 7842, 7: 7716, 46: 6299, 13: 4186, 14: 4066, 0: 3360, 2: 3084, 19: 2132, 24: 841, 21: 169, 22: 169})

20News Natural Data Distribution:
it is split by number of document in this dataset so every single index in attributes only has size one

SQuad 1.1 Natural Data Distribution:
it is split by number of document in this dataset so every single index in attributes only has size one

## Data Format

### 20news
X -> (array) [data_size, source_max_sequence_length] # source inputs

Y -> (array) [data_size, target_max_sequence_length] # target outputs

source_max_sequence_length -> (int) [] # maximum sequence length for source inputs(also can be set up by user)

target_max_sequence_length -> (int) [] # maximum sequence length for target outputs(also can be set up by user)

source_sequence_length -> (array) [data_size] # original sequence lengths for source inputs

target_sequence_length -> (array) [data_size] # original sequence lengths for target outputs

vocab -> (dict) [vocab_size] # vocabulary of inputs

label_vocab -> (dict) [label_vocab_size] # vocabulary of outputs

### AGnews

X -> (array) [data_size, source_max_sequence_length] # source inputs

Y -> (array) [data_size, target_max_sequence_length] # target outputs

source_max_sequence_length -> (int) [] # maximum sequence length for source inputs(also can be set up by user)

target_max_sequence_length -> (int) [] # maximum sequence length for target outputs(also can be set up by user)

source_sequence_length -> (array) [data_size] # original sequence lengths for source inputs

target_sequence_length -> (array) [data_size] # original sequence lengths for target outputs

vocab -> (dict) [vocab_size] # vocabulary of inputs

label_vocab -> (dict) [label_vocab_size] # vocabulary of outputs

### Stanford Sentiment Treebank v2(SST-2)

X -> (array) [data_size, source_max_sequence_length] # source inputs

Y -> (array) [data_size, target_max_sequence_length] # target outputs

source_max_sequence_length -> (int) [] # maximum sequence length for source inputs(also can be set up by user)

target_max_sequence_length -> (int) [] # maximum sequence length for target outputs(also can be set up by user)

source_sequence_length -> (array) [data_size] # original sequence lengths for source inputs

target_sequence_length -> (array) [data_size] # original sequence lengths for target outputs

vocab -> (dict) [vocab_size] # vocabulary of inputs

label_vocab -> (dict) [label_vocab_size] # vocabulary of outputs

### Sentiment140

X -> (array) [data_size, source_max_sequence_length] # source inputs

Y -> (array) [data_size, target_max_sequence_length] # target outputs

source_max_sequence_length -> (int) [] # maximum sequence length for source inputs(also can be set up by user)

target_max_sequence_length -> (int) [] # maximum sequence length for target outputs(also can be set up by user)

source_sequence_length -> (array) [data_size] # original sequence lengths for source inputs

target_sequence_length -> (array) [data_size] # original sequence lengths for target outputs

vocab -> (dict) [vocab_size] # vocabulary of inputs

label_vocab -> (dict) [label_vocab_size] # vocabulary of outputs

### SemEval2010Task8

X -> (array) [data_size, source_max_sequence_length] # source inputs

Y -> (array) [data_size, target_max_sequence_length] # target outputs

source_max_sequence_length -> (int) [] # maximum sequence length for source inputs(also can be set up by user)

target_max_sequence_length -> (int) [] # maximum sequence length for target outputs(also can be set up by user)

source_sequence_length -> (array) [data_size] # original sequence lengths for source inputs

target_sequence_length -> (array) [data_size] # original sequence lengths for target outputs

vocab -> (dict) [vocab_size] # vocabulary of inputs

label_vocab -> (dict) [label_vocab_size] # vocabulary of outputs

### SQuAD_1.1

document_X -> (array) [data_size, max_document_length] # source inputs documents

question_X -> (array) [data_size, max_question_length] # source inputs question

Y -> (array) [data_size, 2] # target answer indices which indicate the start and the end of the target

question_id -> (array) [data_size, 1] # question id correstpond to each answer in Y 

document_max_sequence_length -> (int) [] # maximum sequence length for source document inputs(also can be set up by user)

question_max_sequence_length -> (int) [] # maximum sequence length for question outputs(also can be set up by user)

source_sequence_length -> (array) [data_size] # original sequence lengths for source documents

question_sequence_length -> (array) [data_size] # original sequence lengths for source questions

vocab -> (dict) [vocab_size] # vocabulary of inputs 

question_vocab -> (dict) [question_vocab_size] # vocabulary of questions 

### Cornell Movie
X -> (array) [data_size, source_max_sequence_length] # source inputs

Y -> (array) [data_size, target_max_sequence_length] # target outputs

history -> (array) [data_size, history_max_sequence_length] # history inputs

source_max_sequence_length -> (int) [] # maximum sequence length for source inputs(also can be set up by user)

target_max_sequence_length -> (int) [] # maximum sequence length for target outputs(also can be set up by user)

history_max_sequence_length -> (int) [] # maximum sequence length for history inputs(also can be set up by user)

source_sequence_length -> (array) [data_size] # original sequence lengths for source inputs

target_sequence_length -> (array) [data_size] # original sequence lengths for target outputs

history_sequence_length -> (array) [data_size] # original sequence lengths for history inputs

vocab -> (dict) [vocab_size] # vocabulary of all inputs
​
### CNN DailyMail
X -> (array) [data_size, source_max_sequence_length] # source inputs

Y -> (array) [data_size, target_max_sequence_length] # target outputs

source_max_sequence_length -> (int) [] # maximum sequence length for source inputs(also can be set up by user)

target_max_sequence_length -> (int) [] # maximum sequence length for target outputs(also can be set up by user)

source_sequence_length -> (array) [data_size] # original sequence lengths for source inputs

target_sequence_length -> (array) [data_size] # original sequence lengths for target outputs

source_vocab -> (dict) [vocab_size] # vocabulary of source inputs

target_vocab -> (dict) [vocab_size] # vocabulary of target outputs
​
### WMT
X -> (array) [data_size, source_max_sequence_length] # source inputs

Y -> (array) [data_size, target_max_sequence_length] # target outputs

source_max_sequence_length -> (int) [] # maximum sequence length for source inputs(also can be set up by user)

target_max_sequence_length -> (int) [] # maximum sequence length for target outputs(also can be set up by user)

source_sequence_length -> (array) [data_size] # original sequence lengths for source inputs

target_sequence_length -> (array) [data_size] # original sequence lengths for target outputs

source_vocab -> (dict) [vocab_size] # vocabulary of source inputs

target_vocab -> (dict) [vocab_size] # vocabulary of target outputs
​
### W-NUT 2017
X -> (array) [data_size, max_sequence_length] # source inputs

Y -> (array) [data_size, max_sequence_length] # target outputs

max_sequence_length -> (int) [] # maximum sequence length for all inputs(also can be set up by user)

sequence_length -> (array) [data_size] # original sequence lengths for all inputs

token_vocab -> (dict) [vocab_size] # vocabulary of all inputs

label_vocab -> (dict) [vocab_size] # vocabulary of target labels

### wikigold
X -> (array) [data_size, max_sequence_length] # source inputs

Y -> (array) [data_size, max_sequence_length] # target outputs

max_sequence_length -> (int) [] # maximum sequence length for all inputs(also can be set up by user)

sequence_length -> (array) [data_size] # original sequence lengths for all inputs

token_vocab -> (dict) [vocab_size] # vocabulary of all inputs

label_vocab -> (dict) [vocab_size] # vocabulary of target labels