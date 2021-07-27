---
title: Tratamento de erros para Excel APIs no Microsoft Graph
description: Instruções de tratamento de erros para Excel APIs no Microsoft Graph
author: grangeryy
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 8589b819b2b14af073e9bfe409724473067fe054
ms.sourcegitcommit: a598c09b73e4e43eea5f4aaefea7ffe062e15c39
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/22/2021
ms.locfileid: "53534555"
---
# <a name="error-handling-for-excel-apis-in-microsoft-graph"></a>Tratamento de erros para Excel APIs no Microsoft Graph

Este artigo fornece instruções gerais e sugestões para lidar com erros retornados pelas APIs Excel no Microsoft Graph quando uma solicitação enviada pela API falhar.

## <a name="types-of-error-responses"></a>Tipos de respostas de erro

Excel AS APIs no Microsoft Graph retornar dois tipos de erros. Um deles é a resposta de erro regular, que se parece com o seguinte.

```http
HTTP/1.1 <HTTP status code>
Content-type: application/json

{
  "error": <Error object>
}
```

O segundo é do padrão de operação de longa duração, que pode retornar um código de status HTTP e status de operação no corpo da resposta, como `200 OK` no exemplo a `failed` seguir.

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "status": "failed",
  "error": <Error object>
}
```

Para ambas as respostas de erro, o objeto error tem a seguinte estrutura.

>**Observação:** As respostas de erro seguem a definição na especificação [OData v4](https://docs.oasis-open.org/odata/odata-json-format/v4.0/os/odata-json-format-v4.0-os.html#_Toc372793091) para respostas de erro.

```json
{
  "code": "string",
  "message": "string",
  "innerError": { "@odata.type": "odata.error" }
}
```

O objeto `innerError` pode conter repetidamente mais objetos `innerError` com códigos de erro adicionais, mais específicos. Por exemplo, o objeto error pode conter informações de erro mais detalhadas no código de erro de segundo nível e na mensagem, conforme mostrado.

```json
{
  "code": "Top-level error code",
  "message": "Top-level error message",
  "innerError": {
    "code": "Second-level error code",
    "message": "Second-level error message",
    "innerError": { "@odata.type": "odata.error" }
  }
}
```

## <a name="steps-to-handle-error-responses"></a>Etapas para lidar com respostas de erro

Os Graph microsoft podem usar as etapas a seguir para lidar com erros que ocorrem com Excel APIs.

### <a name="1-determine-whether-it-is-a-long-running-operation-error"></a>1. Determinar se é um erro de operação de longa duração

Antes de lidar com um erro, a primeira etapa é determinar se a resposta de erro é de um padrão de operação em execução longa ou de um padrão regular. Um erro de operação de longa duração retornará um código de status HTTP e `200 OK` o status da operação no corpo da `failed` resposta. Uma resposta de erro regular retornará um código de status de erro HTTP correspondente. 

### <a name="2-parse-second-level-error-code"></a>2. Analisar código de erro de segundo nível

Para o padrão de operação de longa duração e o padrão regular, recomendamos que você siga primeiro as instruções para erros de segundo nível. O código de erro não tem maiúsculas de minúsculas. A tabela a seguir lista instruções para alguns dos erros. O serviço pode adicionar novos códigos de erro a qualquer momento.

| Código                               | Instruções
|:-----------------------------------|:---------------------------------------------
| **accessConflict**   | A solicitação com falha entra em conflito com outros clientes que acessam a lista de trabalho (por exemplo, outro cliente travada na lista de trabalho para edição). O cliente Graph microsoft não deve resendá-lo até que o conflito seja resolvido. Um usuário final pode optar por executar manualmente as mesmas operações com Excel Online para obter mais detalhes sobre o conflito.
| **accessDenied**   | Não é possível executar a operação solicitada (por exemplo, executando alterações em células bloqueadas). O cliente Graph Microsoft não espera que a solicitação com falha seja resendda.
| **badRequestUncategorized**    | Um erro não especificado é encontrado na solicitação com falha. O cliente Graph Microsoft não espera que a solicitação com falha seja resendda.
| **conflictUncategorized**                   | A solicitação com falha entra em conflito com determinado estado do servidor. O cliente Graph microsoft não deve resendá-lo até que o conflito seja resolvido. Um usuário final pode optar por executar manualmente as mesmas operações com Excel Online para obter mais detalhes sobre o conflito.
| **filteredRangeConflict**                   | A operação falhou porque entra em conflito com um intervalo filtrado. O cliente Graph Microsoft não espera que a solicitação com falha seja resendda.
| **forbiddenUncategorized**                    | A solicitação com falha não é permitida. O cliente Graph Microsoft não espera que a solicitação com falha seja resendda. Um usuário final pode optar por executar manualmente as mesmas operações com Excel Online para obter mais detalhes sobre as restrições.
| **gatewayTimeoutUncategorized**         | O serviço não pôde concluir a solicitação dentro do limite de tempo.
| **generalException**         | Ocorreu um erro interno durante o processamento da solicitação. O cliente Graph Microsoft não espera que a solicitação com falha seja resendda.
| **insertDeleteConflict**         | A tentativa de operação de exclusão ou inserção resultou em um conflito. O cliente Graph Microsoft não espera que a solicitação com falha seja resendda. Um usuário final pode optar por executar manualmente as mesmas operações com Excel Online para obter mais detalhes sobre o conflito.
| **internalServerErrorUncategorized**       | Ocorreu um erro não especificado. O cliente Graph Microsoft não espera que a solicitação com falha seja resendda. Se uma sessão for especificada na solicitação com falha, também não será esperado mais acesso à sessão.
| **invalidArgument**         | O argumento é inválido, está ausente ou tem um formato incorreto. O cliente Graph Microsoft não espera que a solicitação com falha seja resendda.
| **invalidReference**         | Esta referência não é válida para a operação atual. O cliente Graph Microsoft não espera que a solicitação com falha seja resendda.
| **invalidSessionAccessConflict**             | A sessão especificada na solicitação é inválida devido a conflitos com outros clientes que estão acessando a lista de trabalho (por exemplo, outro cliente travada na lista de trabalho para edição). Não é esperado mais acesso à sessão especificada na solicitação com falha. A recriação de sessões com a mesma **solicitação createSession** não é esperada até que o conflito seja resolvido. Recriar sessões com uma **solicitação createSession** diferente pode ou não ser bem-sucedida. Um usuário final pode optar por executar manualmente as mesmas operações com Excel Online para obter mais detalhes sobre o conflito.
| **invalidSessionAuthentication**         | A sessão especificada na solicitação é inválida devido a um erro de autenticação. Não é esperado mais acesso à sessão especificada na solicitação com falha. A recriação de sessões com a mesma **solicitação createSession** não é esperada até que as informações de autenticação apropriadas são fornecidas.
| **invalidSessionNotFound**         | A sessão especificada na solicitação é inválida porque a workbook não pode ser encontrada. Não é esperado mais acesso à sessão especificada na solicitação com falha. Não é esperado recriar sessões com a mesma **solicitação createSession.**
| **invalidSessionReCreatable**             | A sessão especificada na solicitação não existe ou é inválida devido a um erro transitório. O cliente Graph microsoft pode tentar recriar uma sessão e retomar o trabalho. Não é esperado mais acesso à sessão especificada na solicitação com falha.
| **invalidSessionRestricted**          | A sessão especificada na solicitação é inválida devido a configurações de serviço ou restrições. Não é esperado mais acesso à sessão especificada na solicitação com falha. A recriação de sessões com a mesma solicitação **createSession** não é esperada até que as restrições ou configurações que bloqueiam as alterações da solicitação. Recriar sessões com uma **solicitação createSession** diferente pode ou não ser bem-sucedida. Um usuário final pode optar por executar manualmente as mesmas operações com o Excel Online para obter mais detalhes das restrições.
| **invalidSessionUnexpected**                | A sessão especificada na solicitação é inválida devido a um problema inesperado. Não é esperado mais acesso à sessão especificada na solicitação com falha. Não é esperado recriar sessões com a mesma **solicitação createSession.** Recriar sessões com uma **solicitação createSession** diferente pode ou não ser bem-sucedida.
| **invalidSessionUnsupportedWorkbook**              | A sessão especificada na solicitação é inválida porque a workbook contém recursos não compatíveis ou excede o limite de tamanho. Normalmente, os fatores sem suporte são introduzidos por outro cliente acessando a lista de trabalho. Não é esperado mais acesso à sessão especificada na solicitação com falha. A recriação de sessões com a mesma **solicitação createSession** não é esperada até que os fatores sem suporte sejam removidos. Recriar sessões com uma solicitação createSession diferente pode ou não ser bem-sucedida. Um usuário final pode optar por executar manualmente as mesmas operações com o Excel Online para obter mais detalhes dos fatores sem suporte ou com a área de trabalho Excel onde a workbook pode ser suportada.
| **itemAlreadyExists**         | O recurso que está sendo criado já existe. O cliente Graph Microsoft não espera que a solicitação com falha seja resendda.
| **itemNotFound**         | O recurso solicitado não existe. O cliente Graph Microsoft não espera que a solicitação com falha seja resendda.
| **methodNotAllowed**         | O método HTTP especificado na solicitação não é permitido no recurso. O cliente Graph Microsoft não espera que a solicitação com falha seja resendda.
| **methodNotAllowedUncategorized**              | O método HTTP especificado na solicitação não é permitido no recurso. O cliente Graph Microsoft não espera que a solicitação com falha seja resendda.
| **nonBlankCellOffSheet**         | Não é possível inserir novas células porque ela empurraria células não vazias para fora do final da planilha. O cliente Graph Microsoft não espera que a solicitação com falha seja resendda. Um usuário final pode excluir linhas ou colunas para dar espaço para que o conteúdo seja inserido e tente novamente.
| **notFoundUncategorized**             | O recurso solicitado não pode ser encontrado. O cliente Graph Microsoft não espera que a solicitação com falha seja resendda.
| **notImplementedUncategorized**            | O recurso solicitado não está implementado no momento. O cliente Graph Microsoft não espera que a solicitação com falha seja resendda.
| **payloadTooLargeUncategorized**              | A carga de solicitação excede o limite de tamanho. O cliente Graph Microsoft não espera que a solicitação com falha seja resendda.
| **rangeExceedsLimit**         | A contagem de células no intervalo excedeu o número máximo suportado. O cliente Graph microsoft pode tentar enviar uma solicitação com tamanho de intervalo menor. Para obter mais informações, consulte limites de recursos e [otimização de desempenho para Office de complementos](/office/dev/add-ins/concepts/resource-limits-and-performance-optimization#excel-add-ins).
| **requestAborted**         | A solicitação foi anulada durante o tempo de funcionamento, o que geralmente foi causado pelo cálculo de longo tempo de funções na manual de trabalho. O cliente Graph Microsoft não espera que a solicitação com falha seja resendda.
| **serviceUnavailableUncategorized**      | O serviço está temporariamente indisponível ou está sobrecarregado. O cliente Graph Microsoft não deve resendá-lo até que a duração de recarga especificada seja aprovada.
| **tooManyRequestsUncategorized**             | A solicitação com falha excede determinada limitação de frequência. O cliente Graph Microsoft não deve resendá-lo até que a duração de recarga especificada seja aprovada.
| **transientFailure**           | A solicitação falhou devido a um erro transitório. O cliente Graph Microsoft não deve resendá-lo até que a duração de recarga especificada seja aprovada.
| **unauthorizedUncategorized**         | As informações de autenticação necessárias para o recurso estão ausentes ou inválidas. O cliente Graph Microsoft não espera que a solicitação com falha seja resendda.
| **unsupportedOperation**         | Não há suporte para a operação que está sendo tentada. O cliente Graph Microsoft não espera que a solicitação com falha seja resendda.
| **unsupportedWorkbook**         | A solicitação falhou. A workbook contém recursos sem suporte ou excede o limite de tamanho. O cliente Graph microsoft não é esperado para reendá-lo até que os fatores sem suporte sejam removidos.

>**Observação:** Para o padrão regular, a solicitação com falha é definida como a solicitação correspondente à resposta. Para o padrão de operação de longa duração, a solicitação com falha é a que dispara a operação com falha.

### <a name="3-parse-the-top-level-error-code"></a>3. Analisar o código de erro de nível superior

Se você não conseguir encontrar o código de [](workbook-error-codes.md#detailed-error-code) erro de segundo nível listado no tópico Códigos de erro detalhados, recomendamos que você siga as instruções fornecidas para erros de nível superior. Os códigos de erro de nível superior são vinculados ao código de status e você pode tomar medidas de acordo com os códigos de status correspondentes. Para obter detalhes sobre códigos de erro de nível superior e mensagens, consulte [Códigos de erro](workbook-error-codes.md#error-code).

### <a name="4-parse-the-status-code"></a>4. Analisar o código de status

Se o código de erro encontrado não estiver na lista de segundo nível ou na lista de nível superior, recomendamos que você tome medidas de acordo com o código de status HTTP.

### <a name="5-error-recovery-cooldown"></a>5. Recarga de recuperação de erros

Para algumas das respostas no padrão regular, uma duração de recarga de recuperação em segundos pode ser fornecida por meio de `Retry-After` um header. Quando uma duração de recarga de recuperação está presente, o cliente do Microsoft Graph não é esperado para enviar qualquer solicitação de acompanhamento antes que a duração especificada passe.

## <a name="special-case-handling"></a>Tratamento de casos especiais

Para solicitações de sessão [,](excel-manage-sessions.md#request-types)se você encontrar um ou erro, quando um código de erro de segundo nível for listado em Códigos de erro detalhados, analisar o código de segundo nível e seguir as instruções correspondentes; caso `502/badGateway` `503/serviceUnavailable` contrário, reconmmendemos [](workbook-error-codes.md#detailed-error-code)que você recrie a sessão diretamente.
<!-- {
  "type": "#page.annotation",
  "description": "Error handling in Excel Graph.",
  "keywords": "error response, error object, error codes, innerError, error handling",
  "section": "documentation",
  "tocPath": ""
} -->
