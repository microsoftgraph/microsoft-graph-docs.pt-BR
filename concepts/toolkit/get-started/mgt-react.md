---
title: Componentes de reagir do Microsoft Graph Toolkit
description: O Microsoft Graph Toolkit reajam Components ( `mgt-react` ) permite que os desenvolvedores de reagir usem o Microsoft Graph Toolkit em seus aplicativos de reagem.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 6781a894e451e2c4751f151beddcacf4e0cdb608
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/11/2020
ms.locfileid: "49658226"
---
# <a name="microsoft-graph-toolkit-react-components"></a>Componentes de reagir do Microsoft Graph Toolkit

O Microsoft Graph Toolkit reajam Components ( `mgt-react` ) permite que os desenvolvedores de reagir usem o Microsoft Graph Toolkit em seus aplicativos de reagem. A biblioteca envolve todos os componentes do Microsoft Graph Toolkit e os exporta como componentes de reagir.

## <a name="what-components-can-i-use"></a>Quais componentes eu posso usar?

A biblioteca é gerada automaticamente a partir do Microsoft Graph Toolkit Web Components e todos os componentes estão disponíveis como componentes de reagir.

Os nomes dos componentes de reagir estão no PascalCase e não incluem o `Mgt` prefixo. Por exemplo, o `mgt-person` componente está disponível como `Person` , e o `mgt-people-picker` componente está disponível como `PeoplePicker` .

## <a name="installation"></a>Instalação 

Para instalar o, use um dos seguintes comandos.

```bash
npm install @microsoft/mgt-react
```

ou

```bash
yarn add @microsoft/mgt-react
```

## <a name="usage"></a>Uso

Todos os componentes estão disponíveis por meio do pacote NPM e são nomeados usando o PascalCase. Para usar um componente, primeiro importe-o na parte superior.

```tsx
import { Person } from '@microsoft/mgt-react';
```

Agora você pode usar `Person` qualquer lugar no seu JSX como um componente de reagir normal.

```tsx
<Person personQuery="me" />
```

Todos os eventos e propriedades mapeiam exatamente como estão definidos na documentação do componente.

Por exemplo, você pode definir a `personDetails` propriedade para um objeto:

```jsx
const App = (props) => {
  const personDetails = {
    displayName: 'Bill Gates',
  };

  return <Person personDetails={personDetails}></Person>;
};
```

Ou registre um manipulador de eventos:

```jsx
import { PeoplePicker, People } from '@microsoft/mgt-react';

const App = (props) => {
  const [people, setPeople] = useState([]);

  const handleSelectionChanged = (e) => {
    setPeople(e.target.selectedPeople);
  };

  return
    <div>
      <PeoplePicker selectionChanged={handleSelectionChanged} />
      Selected People: <People people={people} />
    </div>;
};
```

## <a name="templates"></a>Modelos

A maioria dos componentes do kit de ferramentas do Microsoft Graph [oferece suporte](../customize-components/templates.md) a `mgt-react` modelos e permite que você use o reagir à gravação de modelos.

Por exemplo, para criar um modelo a ser usado para renderizar eventos no `mgt-agenda` componente, primeiro defina um componente a ser usado para renderizar um evento:

```tsx
import { MgtTemplateProps } from '@microsoft/mgt-react';

const MyEvent = (props: MgtTemplateProps) => {
  const { event } = props.dataContext;
  return <div>{event.subject}</div>;
};
```

Em seguida, use-o como um filho do componente disposto e defina o modelo prop para `event` .

```tsx
import { Agenda } from '@microsoft/mgt-react';

const App = (props) => {
  return <Agenda>
    <MyEvent template="event">
  </Agenda>
}
```

A `template` prop permite que você especifique qual modelo substituir. Nesse caso, o `MyEvent` componente será repetido para cada evento e o `event` objeto será passado como parte da `dataContext` prop.

## <a name="see-also"></a>Também consulte

* [Introdução ao Microsoft Graph Toolkit em reagir](./use-toolkit-with-react.md)
* [Saiba mais sobre provedores de autenticação](../providers/providers.md)
