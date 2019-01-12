---
title: Gerenciar sessões e persistências no Excel usando o Microsoft Graph
description: Se o aplicativo precisar realizar mais do que uma ou duas chamadas à API do Excel, você deve criar uma sessão e passar a ID da sessão com cada solicitação. A presença de uma ID de sessão na solicitação garante que você esteja usando a API do Excel da maneira mais eficiente possível.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 151119a2a2861b64db126c8f49d0b916a6f563e8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27921686"
---
# <a name="manage-sessions-and-persistence-in-excel-with-microsoft-graph"></a>Gerenciar sessões e persistências no Excel usando o Microsoft Graph

Se o aplicativo precisar realizar mais do que uma ou duas chamadas à API do Excel, você deve criar uma sessão e passar a ID da sessão com cada solicitação. A presença de uma ID de sessão na solicitação garante que você esteja usando a API do Excel da maneira mais eficiente possível.

As APIs do Excel podem ser chamadas em um destes três modos:

1. **Sessão persistente** Todas as alterações feitas na pasta de trabalho são persistentes (salvas) na pasta de trabalho. Esse uso da API do Excel é o método mais eficiente e que oferece o melhor desempenho.
2. **Sessão não persistente** As alterações feitas pela API não são salvas na localização de origem. Em vez disso, o servidor back-end do Excel mantém uma cópia temporária do arquivo que reflete as alterações feitas durante essa sessão de API específica. Quando a sessão do Excel expirar, as alterações serão perdidas. Esse modo é útil para aplicativos que precisam fazer uma análise ou obter os resultados de um cálculo ou de uma imagem de gráfico, mas não precisa afetar o estado do documento.
3. **Sem sessão** As chamadas da API não passam um ID de sessão. Os servidores do Excel precisam localizar a cópia do servidor da pasta de trabalho para cada operação. Essa não é uma maneira eficiente para chamar a API do Excel, mas ela é adequada para fazer certos tipos de solicitações isoladas.

Para representar a sessão na API, use o cabeçalho `workbook-session-id: {session-id}`.

>**Observação:** o cabeçalho de sessão não é obrigatório para uma API do Excel funcionar. No entanto, recomendamos que você use o cabeçalho de sessão para melhorar o desempenho. Se você não usar um cabeçalho de sessão, as alterações feitas durante a chamada à API _serão_ mantidas como persistentes no arquivo.  

## <a name="next-step"></a>Próxima etapa
Para saber como criar e usar sessões, confira o [tópico de referência de criação de sessão](/graph/api/workbook-createsession?view=graph-rest-1.0).

## <a name="see-also"></a>Confira também
* [Gravar em uma pasta de trabalho do Excel usando o Microsoft Graph](excel-write-to-workbook.md)
* [Usar funções de pasta de trabalho do Excel com o Microsoft Graph](excel-use-functions.md)
* [Atualizar um formato de intervalo no Excel com o Microsoft Graph](excel-update-range-format.md)
* [Exibir uma imagem do gráfico do Excel com o Microsoft Graph](excel-display-chart-image.md)
* [Usar a API REST do Excel](/graph/api/resources/excel?view=graph-rest-1.0)
