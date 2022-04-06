---
title: Componentes Graph Toolkit React Microsoft
description: Os componentes Graph Toolkit React microsoft (`mgt-react`) permitem que React desenvolvedores usem o microsoft Graph Toolkit em seus React aplicativos.
ms.localizationpriority: medium
author: sebastienlevert
ms.openlocfilehash: 4dff722faf3f61b4ed9832c2389b674d9bf1a444
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2022
ms.locfileid: "64588999"
---
# <a name="microsoft-graph-toolkit-react-components"></a>Componentes Graph Toolkit React Microsoft

Os componentes Graph Toolkit React microsoft (`mgt-react`) permitem que React desenvolvedores usem o microsoft Graph Toolkit em seus React aplicativos. A biblioteca quebra todos os componentes Graph Toolkit microsoft e os exporta como React componentes.

## <a name="what-components-can-i-use"></a>Quais componentes posso usar?

A biblioteca é automaticamentegenerada a partir dos componentes da Web do Microsoft Graph Toolkit e todos os componentes estão disponíveis como React componentes.

Os nomes dos componentes React estão em PascalCase e não incluem o `Mgt` prefixo. Por exemplo, o `mgt-person` componente está disponível como `Person`, e o `mgt-people-picker` componente está disponível como `PeoplePicker`.

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

Por exemplo, você pode definir a propriedade `personDetails` como um objeto:

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

A maioria dos Graph Toolkit microsoft [suportam a tentação](../customize-components/templates.md) `mgt-react` e permite que você use React para gravar modelos.

Por exemplo, para criar um modelo `mgt-agenda` a ser usado para renderizar eventos no componente, primeiro defina um componente a ser usado para renderizar um evento:

```tsx
import { MgtTemplateProps } from '@microsoft/mgt-react';

const MyEvent = (props: MgtTemplateProps) => {
  const { event } = props.dataContext;
  return <div>
    {event.subject}<br />
    {event.attendees
      .map((attendee: any) => attendee.emailAddress.name)
      .join(', ')}
  </div>;
};
```

Em seguida, use-o como um filho do componente empacotado e de definir o modelo prop como `event`.

```tsx
import { Agenda } from '@microsoft/mgt-react';

const App = (props) => {
  return <Agenda>
    <MyEvent template="event">
  </Agenda>
}
```

O `template` prop permite especificar qual modelo substituir. Nesse caso, o `MyEvent` componente será repetido para cada evento e `event` o objeto será passado como parte do `dataContext` prop.

## <a name="see-also"></a>Confira também

* [Introdução com o microsoft Graph Toolkit no React](./use-toolkit-with-react.md)
* [Saiba mais sobre provedores de autenticação](../providers/providers.md)
