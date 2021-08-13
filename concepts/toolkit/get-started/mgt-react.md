---
title: Componentes Graph Toolkit React Microsoft
description: Os componentes Graph Toolkit React microsoft ( ) permitem que React `mgt-react` desenvolvedores usem o microsoft Graph Toolkit em seus React aplicativos.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 89225af263c4c8f1cb29b7f6bb02dff6b6badbe379af510f90bed821935be047
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54225675"
---
# <a name="microsoft-graph-toolkit-react-components"></a>Componentes Graph Toolkit React Microsoft

Os componentes Graph Toolkit React microsoft ( ) permitem que React `mgt-react` desenvolvedores usem o microsoft Graph Toolkit em seus React aplicativos. A biblioteca quebra todos os componentes do Microsoft Graph Toolkit e os exporta como React componentes.

## <a name="what-components-can-i-use"></a>Quais componentes posso usar?

A biblioteca é automaticamentegenerada a partir dos componentes da Web do Microsoft Graph Toolkit e todos os componentes estão disponíveis como React componentes.

Os nomes dos componentes React estão em PascalCase e não incluem o `Mgt` prefixo. Por exemplo, o `mgt-person` componente está disponível como , e o componente está disponível como `Person` `mgt-people-picker` `PeoplePicker` .

## <a name="installation"></a>Instalação 

Para instalar, use um dos seguintes comandos.

```bash
npm install @microsoft/mgt-react
```

ou

```bash
yarn add @microsoft/mgt-react
```

## <a name="usage"></a>Uso

Todos os componentes estão disponíveis por meio do pacote npm e são nomeados usando PascalCase. Para usar um componente, primeiro importe-o na parte superior.

```tsx
import { Person } from '@microsoft/mgt-react';
```

Agora você pode usar `Person` em qualquer lugar do JSX como um componente React regular.

```tsx
<Person personQuery="me" />
```

Todas as propriedades e eventos mapeiam exatamente como são definidos na documentação do componente.

Por exemplo, você pode definir a `personDetails` propriedade como um objeto:

```jsx
const App = (props) => {
  const personDetails = {
    displayName: 'Bill Gates',
  };

  return <Person personDetails={personDetails}></Person>;
};
```

Ou, registre um manipulador de eventos:

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

A maioria dos Graph Toolkit microsoft [suporta a tentação](../customize-components/templates.md) e permite que você use React `mgt-react` para gravar modelos.

Por exemplo, para criar um modelo a ser usado para renderizar eventos no componente, primeiro defina um componente a ser usado para `mgt-agenda` renderizar um evento:

```tsx
import { MgtTemplateProps } from '@microsoft/mgt-react';

const MyEvent = (props: MgtTemplateProps) => {
  const { event } = props.dataContext;
  return <div>{event.subject}</div>;
};
```

Em seguida, use-o como um filho do componente empacotado e de definir o modelo prop como `event` .

```tsx
import { Agenda } from '@microsoft/mgt-react';

const App = (props) => {
  return <Agenda>
    <MyEvent template="event">
  </Agenda>
}
```

O `template` prop permite especificar qual modelo substituir. Nesse caso, o componente será repetido para cada evento e o `MyEvent` objeto será passado como parte do `event` `dataContext` prop.

## <a name="see-also"></a>Confira também

* [Começar a trabalhar com o microsoft Graph Toolkit no React](./use-toolkit-with-react.md)
* [Saiba mais sobre provedores de autenticação](../providers/providers.md)
