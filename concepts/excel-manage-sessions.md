---
title: Gerenciar sessões e persistência no Excel
description: Saiba como usar a API do Excel no Microsoft Graph da maneira mais eficiente possível. Saiba mais sobre os três modos para chamar as APIs e os tipos de solicitação relacionados.
ms.localizationpriority: medium
author: lumine2008
ms.prod: excel
ms.openlocfilehash: b2b38c20f3ae1613d9330271cd73af56bb7d33c8
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66440828"
---
# <a name="manage-sessions-and-persistence-in-excel"></a>Gerenciar sessões e persistência no Excel

Se o aplicativo precisar fazer mais de uma ou duas chamadas para a API do Excel no Microsoft Graph, crie uma sessão e passe a ID da sessão com cada solicitação. A presença de uma ID de sessão nas solicitações garante que você está usando a API do Excel da maneira mais eficiente possível.

As APIs do Excel podem ser chamadas em um destes três modos:

- **Sessão persistente:** Todas as alterações feitas na pasta de trabalho são persistidas (salvas) na pasta de trabalho. Esse uso da API do Excel é o método mais eficiente e que oferece o melhor desempenho.

- **Sessão não persistente:** As alterações feitas pela API não são salvas no local de origem. Em vez disso, o servidor back-end do Excel mantém uma cópia temporária do arquivo que reflete as alterações feitas durante essa sessão de API específica. Quando a sessão do Excel expirar, as alterações serão perdidas. Esse modo é útil para aplicativos que precisam fazer uma análise ou obter os resultados de um cálculo ou de uma imagem de gráfico, mas não precisa afetar o estado do documento.

- **Sem sessão:** As chamadas à API não passam uma ID de sessão. Os servidores do Excel devem localizar a cópia da pasta de trabalho do servidor para cada operação. Essa não é uma maneira eficiente para chamar a API do Excel, mas ela é adequada para fazer certos tipos de solicitações isoladas.

Para representar a sessão na API, use o cabeçalho `workbook-session-id: {session-id}`.

> [!NOTE]
> O cabeçalho da sessão não é necessário para que uma API do Excel funcione. No entanto, recomendamos que você use o cabeçalho de sessão para melhorar o desempenho. Se você não usar um cabeçalho de sessão, as alterações feitas durante a chamada da API _serão_ mantidas como persistentes no arquivo.  

## <a name="request-types"></a>Tipos de solicitação

O [tratamento de erro](workbook-error-handling.md) sugerido para APIs do Excel baseia-se no tipo de solicitação, no código de erro e no código de status. A seguir estão os tipos de solicitação:

- **Solicitação CreateSession:** Usado para criar uma sessão persistente ou não persistente. Em uma resposta bem-sucedida, a ID da sessão será retornada na **propriedade ID** no corpo da resposta. Para obter detalhes, consulte [Criar sessão](/graph/api/workbook-createsession).
- **Solicitação com sessão:** Solicitações subsequentes que seguem uma solicitação CreateSession. Geralmente, eles incluem `workbook-session-id: {session-id}` um cabeçalho. A exceção é uma solicitação de status de sondagem, que usa o padrão de operação de execução longa. Para obter detalhes, [consulte Trabalhar com APIs que levam muito tempo para serem concluídas](./workbook-best-practice.md#work-with-apis-that-take-a-long-time-to-complete).
- **Solicitação sem sessão:** Usado no modo sem sessão. Essas solicitações não têm um `workbook-session-id: {session-id}` cabeçalho.  

## <a name="next-steps"></a>Próximas etapas

Para saber como criar e usar sessões, confira o [tópico de referência de criação de sessão](/graph/api/workbook-createsession).

## <a name="see-also"></a>Confira também

* [Gravar em uma pasta de trabalho do Excel usando o Microsoft Graph](excel-write-to-workbook.md)
* [Usar funções de pasta de trabalho do Excel com o Microsoft Graph](excel-use-functions.md)
* [Atualizar um formato de intervalo no Excel com o Microsoft Graph](excel-update-range-format.md)
* [Exibir uma imagem do gráfico do Excel com o Microsoft Graph](excel-display-chart-image.md)
* [Usar a API REST do Excel](/graph/api/resources/excel)