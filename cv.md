# Talap Ali

**Phone:** +7 747 *** **\*\*\
**Email:** talapali@mail.ru

# About myself

My goal for this trip is to be fronted developer. I'm appreciate with this stuff and it'd be very cool. Since I love programming I will be on the top of my field in particular year.

# Skills

* Python
* C++
* JavaScript
* HTML
* CSS

# Code examples

### (6kyu) Decode the Morse code
**Link to task:** [Codewars](https://www.codewars.com/kata/54b724efac3d5402db00065e)
```
decodeMorse = function(morseCode){
  let decode = '';
  morseCode = morseCode.trim().split(' ');
  for (let i = 0; i < morseCode.length; i++) {
    if (morseCode[i] === '') {
      decode += ' ';
      i++;
    } else {
      decode += MORSE_CODE[morseCode[i]];
    }
  }
  return decode;
}
```

### (4kyu) Decode the Morse code, advanced
**Link to task:** [Codewars](https://www.codewars.com/kata/54b72c16cd7f5154e9000457)
```
var decodeBits = function(bits){
    if (bits.startsWith('0')) bits = bits.substring(bits.search('1'));
    if (bits.endsWith('0')) {
        let i = bits.length - 1;
        while (bits[i] === '0') {
            i--;
        }
        bits = bits.substring(0, i + 1);
    }
    const times = [];
    for (let i = 0; i < bits.length;) {
        let digit = bits[i];
        let count = digit === '1' ? bits.substring(i).search('0') : bits.substring(i).search('1');
        if (count === -1) count = bits.length - i;
        times.push(bits.substr(i, count));
        i += count;
    }  
    let str = '';
    let timeUnit = times[0].length;
    times.forEach(unit => {
        if (timeUnit > unit.length) timeUnit = unit.length;
    });
    for (const unit of times) {
        let digit = unit[0];
        let count = unit.length;
        switch (count) {
            case timeUnit:
                str += digit === '1' ? '.' : '';
                break;
            case timeUnit*3:
                str += digit === '1' ? '-' : ' ';
                break;
            default:
                str += '   ';
        }
    }
    return str;
}

var decodeMorse = function(morseCode){
  return morseCode
    .trim()
    .split(/  | /)
    .map(e => MORSE_CODE[e] || ' ')
    .join('');
}
```

# Work experience

### Landing page
*Languages:* HTML, CSS\
*Link:* [GitHub](https://github.com/Bauyrsaq/Landing-Page)

### Rock paper scissors
*Languages:* JavaScript, HTML, CSS\
*Link:* [GitHub](https://github.com/Bauyrsaq/rock-paper-scissors)

# Education

* Secondary education
* [Программирование на Python](https://stepik.org/course/67/info)
* [Python: основы и применение](https://stepik.org/course/512/syllabus?auth=login)

# English

A2-B1