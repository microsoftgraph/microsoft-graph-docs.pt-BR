---
title: Recursos de seleção e filtragem de usuários na Conexão de Dados do Microsoft Graph
description: Você pode utilizar o Microsoft Graph Data Connect para selecionar os usuários para os quais deseja extrair dados e incluir filtros para limitar os dados retornados.
author: fercobo-msft
ms.localizationpriority: high
ms.prod: data-connect
ms.openlocfilehash: bcdbfe58b628ee0f431a529d8a3372c6c1c9266e
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2022
ms.locfileid: "66094022"
---
# <a name="user-selection-and-filtering-capabilities-in-microsoft-graph-data-connect"></a>Recursos de seleção e filtragem de usuários na Conexão de Dados do Microsoft Graph

Você pode utilizar o Microsoft Graph Data Connect para selecionar os usuários para os quais deseja extrair dados e incluir filtros para limitar os dados retornados. Este artigo descreve as opções que a Conexão de Dados suporta para filtragem e seleção do usuário.

## <a name="user-selection"></a>Seleção de usuário

Você pode executar pipelines em um conjunto de usuários. As opções para seleção de usuário são as seguintes:

- Todos os usuários da organização
- Até 10 grupos de usuários dentro da organização
- Um conjunto de usuários com base em um predicado com as propriedades de usuário do Azure Active Directory

Especifique a seleção de usuários em OrigemDoConjuntoDeDados da atividade de cópia do Azure Data Factory. Para executar em uma lista de grupos, adicione um novo campo **GruposPermitidos** em **PropriedadesDoTipo** e aplique essa definição para uma lista de até dez **IDs de objeto** de um grupo, separados por vírgulas. Se nenhum grupo for especificado por padrão, os dados serão extraídos para toda a organização.

Para especificar um predicado para executar no locatário inteiro, adicione um novo campo **EscopoDeFiltroUriDoUsuário** em **PropriedadesDoTipo** e o defina no predicado. O formato do predicado deve coincidir com o formato de consulta de APIs do Microsoft Graph. Se você quiser limitar a seleção para os usuários que funcionam no departamento de finanças, você pode usar `https://graph.microsoft.com/v1.0/users?$filter=Department eq 'Finance'`, por exemplo. Se desejar limitar a seleção a um usuário, você pode usar o `https://graph.microsoft.com/v1.0/users?$filter=mail eq 'contosouser1@contoso.com'`.

Sua consulta retornará somente usuários dentro da organização do Microsoft 365 que você está consultando. Caixas de correio de usuários convidados e não usuários não são retornadas.

## <a name="filtering"></a>Filtragem

Você pode limitar os resultados extraídos da sua consulta usando as propriedades DateTime. Dependendo do tipo de dado solicitado, talvez seja necessário um filtro de data e hora. O filtro DateTime é fornecido usando propriedades no SourceDataSet da atividade de cópia do Azure Data Factory. Para especificar um filtro de data e hora, adicione um novo campo **FiltroDeColunaDeData** em **PropriedadesDoTipo** e aplique essa definição para uma das propriedades de suporte à filtragem na tabela a seguir. Em seguida, adicione um **startTime** e **endTime** que representam os valores do DateTime em que a propriedade é filtrada.

Os conjuntos de dados a seguir exigem que um filtro seja fornecido em uma das propriedades de data e hora correspondentes.

| Nome do conjunto de dados                                               | Propriedades de suporte à filtragem                                           |
| ---------------------------------------------------------- | --------------------------------------------------------------------------- |
| BasicDataSet_v0.Event_v0<br>BasicDataSet_v0.Event_v1       | DataeHoraDaCriação<br>DataeHoraDaÚltimaModificação                                     |
| BasicDataSet_v0.Message_v0<br>BasicDataSet_v0.Message_v1   | DataeHoraDaCriação<br>DataeHoraDaÚltimaModificação<br>DataeHoraRecebida<br>DataeHoraEnviada |
| BasicDataSet_v0.SentItem_v0<br>BasicDataSet_v0.SentItem_v1 | DataeHoraDaCriação<br>DataeHoraDaÚltimaModificação<br>DataeHoraRecebida<br>DataeHoraEnviada |

> [!NOTE]
> Os pipelines que solicitam BasicDataSet_v0.CalendarView_v0 também exigem um filtro de data e hora, mas nenhum **dateFilterColumn** é especificado na SourceDataSet. No entanto, são necessários um **startTime** e **endTime**, e somente eventos que começam após o **startTime** e terminam antes do **endTime** são fornecidos.

## <a name="see-also"></a>Confira também

- [Integração com PAM](data-connect-pam.md)
- [Perguntas frequentes sobre a Conexão de Dados](data-connect-faq.md)
