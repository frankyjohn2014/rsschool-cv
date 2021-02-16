# Dmitriy Smolskiy

## Phone: 
+375336105624 
## Email: 
frankyjohn2014@gmail.com

## Summary
Hello, I’m a Dmitriy. I am 27 years old. I aspiring web developer based in Minsk. I have some experience in designing, building and customizing websites. Currently studying «JavaScript/Front-end» at RS School.

## Skills
* HTML, CSS, JavaScript (ES6 +), HTML5, CSS3, React, Redux, Typescript, Babel, Git, Docker;
* C (Microcontrollers AVR, ARM), C# (Unity , WPF), Python (Flask,Django,DRF)

## Code example (latest):
```
export const loginReducer = (email:string, password:string,rememberMe:boolean,captcha:string) => {
    return async (dispatch:any) => {
        let response = await AuthApi.login(email, password, rememberMe, captcha)
            if (response.data.resultCode === 0) {
                dispatch(getAuthData())
            } else {
                if (response.data.resultCode === 10) {
                    dispatch(getCaptchaThunk())
                }
                let ErrMessage = response.data.messages.length > 0 ?  response.data.messages[0] : "Some error"
                dispatch(stopSubmit('login',{_error: ErrMessage}))
        }
    }
}
```

## Education
* **Aviation Equipment** - Belarussian State Academy of Aviation
September 2011 - July 2017
* **Course:** Udemy Uriy Bura React, Udemy ReactJs Vladilen Minin, Coursera Python, Python WebFromMySelf, Udemy React Hooks, Udemy Docker and Docker Compose.

## Language competencies
English: Elementary (A2)