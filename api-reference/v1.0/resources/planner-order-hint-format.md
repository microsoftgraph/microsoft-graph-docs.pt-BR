---
title: Usando dicas de ordenação no Planner
description: '`)'
author: TarkanSevilmis
ms.localizationpriority: medium
ms.prod: planner
doc_type: conceptualPageType
ms.openlocfilehash: ff33069f1427700d0c60bf7300052eb127c37e34
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59044430"
---
# <a name="using-order-hints-in-planner"></a>Usando dicas de ordenação no Planner

Namespace: microsoft.graph

Os objetos no Planner identificam sua ordem de classificação pelas dicas de ordenação. Os valores de dica de ordenação são cadeias de caracteres. Os clientes podem classificar as cadeias de caracteres com base no valor ordinal dos caracteres nelas para identificar a ordem dos itens. Os caracteres são comparados desde o início da cadeia de caracteres, até que uma diferença seja encontrada nos valores ordinais de caracteres ou uma cadeia de caracteres termina, caso em que a cadeia de caracteres mais curta seria classificada antes da mais longa. Os valores podem conter qualquer caractere ordinal entre 32 (espaço) e 126 (`~`)

Por exemplo, um item com dica de ordenação `a` (valor ordinal 97) seria colocado antes de outro item com dica de ordenação `z` (valor ordinal 122). Um item com dica de ordenação `abc` (valores ordinais 97, 98, 99), seriam colocados antes de outro item com dica de ordenação `abd` (valores ordinais 97, 98, 100). Um item com dica de ordenação `a` seria colocado antes de outro item com dica de ordenação `ab` já que todos os caracteres existentes são os mesmos e `a` é mais curto.

Os valores de todas as dicas de ordenação são calculados pelo serviço. O cliente pode reordenar os itens especificando a dica de ordenação do item que foi movido entre dois itens definindo a dica de ordenação do seguinte valor: `<previous order hint> <next order hint>!`, onde `<previous order hint>` deve ser substituído pela dica de ordenação do item que vem antes do novo local desejado e `<next order hint>` deve ser substituído pela dica de ordenação do item que vem depois do novo local desejado. Há um caractere de espaço entre esses valores de dica de ordenação e o valor inteiro tem o sufixo `!`. Se o item não estiver presente, deve ser usada uma cadeia de caracteres vazia. Esse valor também pode ser composto por cálculos anteriores e pode ser usado no cliente para classificar os itens exatamente como as dicas de ordenação retornadas pelo serviço. Depois que o cliente envia esses valores em uma atualização, o serviço calculará um valor curto que classifica no local desejado.

**Observe** que, nos exemplos a seguir, os valores de dica de ordenação reais são cercados por caracteres de aspa simples (`'`) para fins de clareza, no entanto, eles não fazem parte dos dados e não devem ser enviados para o serviço.
 
Por exemplo, considere a seguinte lista de dicas de ordem de classificação:

1. Item 1 (Dica de ordenação: `'5637'`)
2. Item 2 (Dica de ordenação: `'adhg'`)

Colocar um Item 3 antes de um Item 1 e colocar o item 4 entre o Item 1 e o Item 2 e o item 5 depois do Item 2, criaria as seguintes dicas de ordenação no cliente. 

1. Item 3 (Dica de ordenação: `' 5637!'`)
2. Item 1 (Dica de ordenação: `'5637'`)
3. Item 4 (Dica de ordenação: `'5637 adhg!'`)
4. Item 2 (Dica de ordenação: `'adhg'`)
5. Item 5 (Dica de ordenação: `'adhg !'`)

Em seguida, mover o item 1 para o fim da lista geraria:

1. Item 3 (Dica de ordenação: `' 5637!'`)
2. Item 4 (Dica de ordenação: `'5637 adhg!'`)
3. Item 2 (Dica de ordenação: `'adhg'`)
4. Item 5 (Dica de ordenação: `'adhg !'`)
5. Item 1 (Dica de ordenação: `'adhg ! !'`)

Por fim, mover o Item 5 entre o Item 3 e o Item 4 geraria:

1. Item 3 (Dica de ordenação: `' 5637!'`)
2. Item 5 (Dica de ordenação: `' 5637! 5637 adhg!!'`)
3. Item 4 (Dica de ordenação: `'5637 adhg!'`)
4. Item 2 (Dica de ordenação: `'adhg'`)
5. Item 1 (Dica de ordenação: `'adhg ! !'`)

Depois que essas alterações aos valores de dica de ordenação são enviadas para o serviço em solicitações de patch, o serviço calculará valores apropriados que mantém a ordem pretendida pelo cliente. O cliente pode obter os valores imediatamente se a preferência `return=representation` estiver especificada nas solicitações `PATCH`. Os valores do caso acima podem ter a seguinte aparência (os valores reais podem diferir). 

1. Item 3 (Dica de ordenação: `'432b'`)
2. Item 5 (Dica de ordenação: `'6F"#'`)
3. Item 4 (Dica de ordenação: `'7A$6'`)
4. Item 2 (Dica de ordenação: `'adhg'`)
5. Item 1 (Dica de ordenação: `'de5%'`)

Dicas de ordenação podem ser especificadas para criar o primeiro item na lista como `!`, pois nem um item anterior ou próximo existe nesse caso, porém isso é desnecessário, como o serviço gerará automaticamente valores para todos os valores de dica de ordenação nos itens se eles não forem especificados durante a criação do item. O exemplo a seguir ilustra as dicas de ordenação que devem ser usadas ao inserir itens em uma lista anteriormente vazia.
Adicione o primeiro item:

1. Item 1 (Dica de ordenação: `' !'`)

Adicione o segundo item ao topo:

1. Item 2 (Dica de ordenação: `'  !!'`)
2. Item 1 (Dica de ordenação: `' !'`)

Adicione o terceiro item à parte inferior:

1. Item 2 (Dica de ordenação: `'  !!'`)
2. Item 1 (Dica de ordenação: `' !'`)
3. Item 3 (Dica de ordenação: `' ! !'`)








