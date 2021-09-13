---
title: Recursos de seleção e filtragem de usuários na Conexão de Dados do Microsoft Graph
description: Descreve como usar a Conexão de Dados do Microsoft Graph ara selecionar os usuários cujos dados serão extraídos e filtrar os dados retornados.
author: fercobo-msft
ms.localizationpriority: high
ms.prod: data-connect
ms.openlocfilehash: cfe05545a6cfacc08f132be37c54c3a31ccdd62a
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59139181"
---
# <a name="user-selection-and-filtering-capabilities-in-microsoft-graph-data-connect"></a>Recursos de seleção e filtragem de usuários na Conexão de Dados do Microsoft Graph

Você pode usar a Conexão de Dados do Microsoft Graph para selecionar os usuários cujos dados serão extraídos, e para aplicar filtros para limitar os dados retornados. Este artigo descreve as opções que a Conexão de Dados suporta para filtragem e seleção do usuário.

## <a name="user-selection"></a>Seleção de usuário

Você pode executar pipelines em um conjunto de usuários. As opções para seleção de usuário são as seguintes:

- Todos os usuários da organização
- Execução em grupos de até dez usuários da organização
- Um conjunto de usuários com base em um predicado com as propriedades de usuário do Azure Active Directory

Especifique a seleção de usuários em OrigemDoConjuntoDeDados da atividade de cópia do Azure Data Factory. Para executar em uma lista de grupos, adicione um novo campo **GruposPermitidos** em **PropriedadesDoTipo** e aplique essa definição para uma lista de até dez **IDs de objeto** de um grupo, separados por vírgulas. Se nenhum grupo for especificado por padrão, os dados serão extraídos da organização inteira.

Para especificar um predicado para executar no locatário inteiro, adicione um novo campo **EscopoDeFiltroUriDoUsuário** em **PropriedadesDoTipo** e o defina no predicado. O formato do predicado deve coincidir com o formato de consulta de APIs do Microsoft Graph. Se você quiser limitar a seleção para os usuários que funcionam no departamento de finanças, você pode usar `https://graph.microsoft.com/v1.0/users?$filter=Department eq 'Finance'`, por exemplo. Se desejar limitar a seleção a um usuário, você pode usar o `https://graph.microsoft.com/v1.0/users?$filter=mail eq 'contosouser1@contoso.com'`.

A consulta retornará somente usuários dentro da organização do Microsoft 365 que você está pesquisando. Os usuários convidados e caixas de correio que não são de usuários não serão retornadas.

## <a name="filtering"></a>Filtragem

Você pode limitar os resultados extraídos de sua consulta usando as propriedades de data e hora. Dependendo do tipo de dado solicitado, talvez seja necessário um filtro de data e hora. O filtro de data e hora é fornecido usando as propriedades OrigemDoConjuntoDeDados da atividade de cópia do Azure Data Factory. Para especificar um filtro de data e hora, adicione um novo campo **FiltroDeColunaDeData** em **PropriedadesDoTipo** e aplique essa definição para uma das propriedades de suporte à filtragem na tabela a seguir. Em seguida, adicione uma **hora de início** e **hora de término** que representam os valores de data e hora que a propriedade será filtrada.

Os conjuntos de dados a seguir exigem que um filtro seja fornecido em uma das propriedades de data e hora correspondentes.

| Nome do conjunto de dados                                               | Propriedades de suporte à filtragem                                           |
| ---------------------------------------------------------- | --------------------------------------------------------------------------- |
| BasicDataSet_v0.Event_v0<br>BasicDataSet_v0.Event_v1       | DataeHoraDaCriação<br>DataeHoraDaÚltimaModificação                                     |
| BasicDataSet_v0.Message_v0<br>BasicDataSet_v0.Message_v1   | DataeHoraDaCriação<br>DataeHoraDaÚltimaModificação<br>DataeHoraRecebida<br>DataeHoraEnviada |
| BasicDataSet_v0.SentItem_v0<br>BasicDataSet_v0.SentItem_v1 | DataeHoraDaCriação<br>DataeHoraDaÚltimaModificação<br>DataeHoraRecebida<br>DataeHoraEnviada |

> [!NOTE]
> Os pipelines que solicitam BasicDataSet_v0.CalendarView_v0 também exigem um filtro de data e hora, mas nenhum **dateFilterColumn** é especificado na SourceDataSet. No entanto, uma **startTime** e **endTime** são obrigatórios e somente eventos que começam após a **startTime** e que terminam antes da **endTime** são fornecidos.

## <a name="see-also"></a>Confira também

- [Integração com PAM](data-connect-pam.md)
- [Perguntas frequentes sobre a Conexão de Dados](data-connect-faq.md)
