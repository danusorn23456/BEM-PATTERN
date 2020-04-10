# BEM design pattern



### BEM Rules
	block-name__element-name  element-name__mode_value
    
### My Adaption
    block-name__element-name  element-name--mod-name_value //i use this beacuse it easy to read
    
### Block
 	สิ่งที่สามารถอยู่ตัวเดี่ยวๆแล้วมีความหมายที่ชัดเจน เช่น header regiser-form main-content
    
### Element
	ใช่ไม่ได้หากไม่มี base/block มารองรับ เช่น content__card gender__checkbox search-form__input
    
### Modifier
	คุณลักษณะของ block หรือ element เช่น input--red button_submit image--size_large 
    
 
## Example Pattern

### Normal
```html
	<header class="header">
    	<img class="header__logo"/>
        <form class="header__search-form">
        	<input class="header__input"></input>
            <button class="header__button"></button>
        </form>
        <figure class="header__figure"></figure>
        	<img class="header__image"/>
        </div>
    </header>
```

### Adaption
```html
	<header class="header">
    	<img class="header__logo"/>
        <div class="search-form header__earch-form">
        	<input class="searhc-form__input"></input>
            <button class="header__button"></button>
        </div>
        <figure class="header__figure"></figure>
        	<img class="header__image"/>
        </div>
    </header>
```

