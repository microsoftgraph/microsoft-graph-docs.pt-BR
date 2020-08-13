---
title: Tratamento de erros para APIs do Excel no Microsoft Graph
description: Instruções de tratamento de erro para APIs do Excel no Microsoft Graph
author: grangeryy
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 5b8fed4992376247bb57c3c9288cea8f66d36082
ms.sourcegitcommit: 7dcd32f9e959bea2dfd81d9e0d4092f93da43cb7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2020
ms.locfileid: "46658131"
---
# <a name="error-handling-for-excel-apis-in-microsoft-graph"></a>Tratamento de erros para APIs do Excel no Microsoft Graph

Este artigo fornece instruções gerais e sugestões para tratamento de erros que são retornados pelas APIs do Excel no Microsoft Graph quando uma solicitação enviada por meio da API falha.

## <a name="types-of-error-responses"></a>Tipos de respostas de erro

As APIs do Excel no Microsoft Graph retornam dois tipos de erros. Uma é a resposta de erro regular, que é parecida com a seguinte:

```http
HTTP/1.1 <HTTP status code>
Content-type: application/json

{
  "error": <Error object>
}
```

O segundo é do padrão de operação de execução longa, que pode retornar um `200 OK` código de status HTTP e um `failed` status de operação no corpo da resposta, como no exemplo a seguir.

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "status": "failed",
  "error": <Error object>
}
```

Para ambas as respostas de erro, o objeto Error tem a estrutura a seguir.

>**Observação:** As respostas de erro seguem a definição na especificação [OData v4](https://docs.oasis-open.org/odata/odata-json-format/v4.0/os/odata-json-format-v4.0-os.html#_Toc372793091) para respostas de erro.

```json
{
  "code": "string",
  "message": "string",
  "innerError": { "@odata.type": "odata.error" }
}
```

O objeto `innerError` pode conter repetidamente mais objetos `innerError` com códigos de erro adicionais, mais específicos. Por exemplo, o objeto Error pode conter informações de erro mais detalhadas no código de erro de segundo nível e mensagens, conforme mostrado.

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

Os clientes do Microsoft Graph podem usar as etapas a seguir para lidar com os erros que ocorrem com as APIs do Excel.

### <a name="1-determine-whether-it-is-a-long-running-operation-error"></a>1. Determine se é um erro de operação de execução longa

Antes de lidar com um erro, a primeira etapa é determinar se a resposta de erro é de um padrão de operação de execução longa ou normal. Um erro de operação de execução longa retornará um `200 OK` código de status HTTP e um `failed` status de operação no corpo da resposta. Uma resposta de erro regular retornará um código de status de erro HTTP correspondente. 

### <a name="2-parse-second-level-error-code"></a>2. analisar o código de erro de segundo nível

Para o padrão de operação de execução demorada e o padrão normal, recomendamos que você primeiro siga as instruções para erros de segundo nível. O código de erro não diferencia maiúsculas de minúsculas. A tabela a seguir lista as instruções para alguns dos erros. O serviço pode adicionar novos códigos de erro a qualquer momento.

| Código                               | Instruções
|:-----------------------------------|:---------------------------------------------
| **accessConflict**   | A solicitação com falha entra em conflito com outros clientes que acessam a pasta de trabalho (por exemplo, outro cliente bloqueou a pasta de trabalho para edição). O cliente do Microsoft Graph não deve reenviar a solicitação com falha até que o conflito seja resolvido. Um usuário final xN optar por executar manualmente as mesmas operações com o Excel online para obter mais detalhes sobre o conflito.
| **accessDenied**   | Você não pode executar a operação solicitada (por exemplo, realizando alterações em células bloqueadas). O cliente do Microsoft Graph não espera reenviar a solicitação com falha.
| **badRequestUncategorized**    | Um erro não especificado é encontrado na solicitação com falha. O cliente do Microsoft Graph não espera reenviar a solicitação com falha.
| **conflictUncategorized**                   | A solicitação com falha entra em conflito com determinado estado do servidor. O cliente do Microsoft Graph não deve reenviar a solicitação com falha até que o conflito seja resolvido. Um usuário final pode optar por executar manualmente as mesmas operações com o Excel online para obter mais detalhes sobre o conflito.
| **filteredRangeConflict**                   | A operação falhou porque está em conflito com um intervalo filtrado. O cliente do Microsoft Graph não espera reenviar a solicitação com falha.
| **forbiddenUncategorized**                    | A solicitação com falha não é permitida. O cliente do Microsoft Graph não espera reenviar a solicitação com falha. Um usuário final pode optar por executar manualmente as mesmas operações com o Excel online para obter mais detalhes sobre as restrições.
| **gatewayTimeoutUncategorized**         | O serviço não pôde concluir a solicitação dentro do limite de tempo. O cliente do Microsoft Graph não deve reenviar a solicitação com falha até que a duração de cooldown especificada seja aprovada.
| **generalException**         | Ocorreu um erro interno ao processar a solicitação. O cliente do Microsoft Graph não espera reenviar a solicitação com falha.
| **insertDeleteConflict**         | A tentativa de operação de exclusão ou inserção resultou em um conflito. O cliente do Microsoft Graph não espera reenviar a solicitação com falha.
| **internalServerErrorUncategorized**       | Ocorreu um erro não especificado. O cliente do Microsoft Graph não espera reenviar a solicitação com falha. Se uma sessão for especificada na solicitação com falha, o acesso adicional à sessão não será esperado.
| **invalidArgument**         | O argumento é inválido, está ausente ou tem um formato incorreto. O cliente do Microsoft Graph não espera reenviar a solicitação com falha.
| **invalidReference**         | Esta referência não é válida para a operação atual. O cliente do Microsoft Graph não espera reenviar a solicitação com falha.
| **invalidSessionAccessConflict**             | A sessão especificada na solicitação é inválida devido a conflitos com outros clientes que estão acessando a pasta de trabalho (por exemplo, outro cliente bloqueou a pasta de trabalho para edição). Não é esperado acesso adicional à sessão especificada na solicitação com falha. A recriação de sessões com a mesma solicitação **CreateSession** não é esperada até que o conflito seja resolvido. A recriação de sessões com uma solicitação **CreateSession** diferente pode ou não ser bem-sucedida. Um usuário final pode optar por executar manualmente as mesmas operações com o Excel online para obter mais detalhes sobre o conflito.
| **invalidSessionAuthentication**         | A sessão especificada na solicitação é inválida devido a um erro de autenticação. Não é esperado acesso adicional à sessão especificada na solicitação com falha. A recriação de sessões com a mesma solicitação **CreateSession** não é esperada até que as informações apropriadas de autenticação sejam fornecidas.
| **invalidSessionNotFound**         | A sessão especificada na solicitação é inválida porque a pasta de trabalho não pode ser encontrada. Não é esperado acesso adicional à sessão especificada na solicitação com falha. A recriação de sessões com a mesma solicitação **CreateSession** não é esperada.
| **invalidSessionReCreatable**             | A sessão especificada na solicitação não existe ou é inválida devido a um erro transitório. O cliente do Microsoft Graph pode tentar recriar uma sessão e continuar o trabalho. Não é esperado acesso adicional à sessão especificada na solicitação com falha.
| **invalidSessionRestricted**          | A sessão especificada na solicitação é inválida devido a configurações ou restrições de serviço. Não é esperado acesso adicional à sessão especificada na solicitação com falha. A recriação de sessões com a mesma solicitação **CreateSession** não é esperada até que as restrições ou configurações que bloqueiam as alterações de solicitação. A recriação de sessões com uma solicitação **CreateSession** diferente pode ou não ser bem-sucedida. Um usuário final pode optar por executar manualmente as mesmas operações com o Excel online para obter mais detalhes sobre as restrições.
| **invalidSessionUnexpected**                | A sessão especificada na solicitação é inválida devido a um problema inesperado. Não é esperado acesso adicional à sessão especificada na solicitação com falha. A recriação de sessões com a mesma solicitação **CreateSession** não é esperada. A recriação de sessões com uma solicitação **CreateSession** diferente pode ou não ser bem-sucedida.
| **invalidSessionUnsupportedWorkbook**              | A sessão especificada na solicitação é inválida porque a pasta de trabalho contém recursos sem suporte ou excede o limite de tamanho. Normalmente, os fatores sem suporte são introduzidos por outro cliente que esteja acessando a pasta de trabalho. Não é esperado acesso adicional à sessão especificada na solicitação com falha. A recriação de sessões com a mesma solicitação **CreateSession** não é esperada até que os fatores sem suporte sejam removidos. A recriação de sessões com uma solicitação CreateSession diferente pode ou não ser bem-sucedida. Um usuário final pode optar por executar manualmente as mesmas operações com o Excel online para obter mais detalhes dos fatores sem suporte ou com a área de trabalho do Excel onde a pasta de trabalho pode ter suporte.
| **itemAlreadyExists**         | O recurso que está sendo criado já existe. O cliente do Microsoft Graph não espera reenviar a solicitação com falha.
| **itemNotFound**         | O recurso solicitado não existe. O cliente do Microsoft Graph não espera reenviar a solicitação com falha.
| **methodNotAllowed**         | O método HTTP especificado na solicitação não é permitido no recurso. O cliente do Microsoft Graph não espera reenviar a solicitação com falha.
| **methodNotAllowedUncategorized**              | O método HTTP especificado na solicitação não é permitido no recurso. O cliente do Microsoft Graph não espera reenviar a solicitação com falha.
| **nonBlankCellOffSheet**         | Não é possível inserir novas células porque elas empurraram células não vazias para fora do final da planilha. O cliente do Microsoft Graph não espera reenviar a solicitação com falha.
| **notFoundUncategorized**             | O recurso solicitado não pode ser encontrado. O cliente do Microsoft Graph não espera reenviar a solicitação com falha.
| **notImplementedUncategorized**            | O recurso solicitado não foi implementado no momento. O cliente do Microsoft Graph não espera reenviar a solicitação com falha.
| **payloadTooLargeUncategorized**              | A carga de solicitação excede o limite de tamanho. O cliente do Microsoft Graph não espera reenviar a solicitação com falha.
| **rangeExceedsLimit**         | A contagem de células no intervalo excedeu o número máximo com suporte. O cliente do Microsoft Graph pode tentar enviar uma solicitação com tamanho de intervalo menor.
| **requestAborted**         | A solicitação foi anulada durante o tempo de execução, que normalmente era causado por um longo tempo de cálculo de funções na pasta de trabalho. O cliente do Microsoft Graph não espera reenviar a solicitação com falha.
| **serviceUnavailableUncategorized**      | O serviço está temporariamente indisponível ou está sobrecarregado. O cliente do Microsoft Graph não deve reenviar a solicitação com falha até que a duração de cooldown especificada seja aprovada.
| **tooManyRequestsUncategorized**             | A solicitação com falha excede a determinada limitação de frequência. O cliente do Microsoft Graph não deve reenviar a solicitação com falha até que a duração de cooldown especificada seja aprovada.
| **transientFailure**           | A solicitação falhou devido a um erro transitório. O cliente do Microsoft Graph não deve reenviar a solicitação com falha até que a duração de cooldown especificada seja aprovada.
| **unauthorizedUncategorized**         | As informações de autenticação necessárias para o recurso estão ausentes ou são inválidas. O cliente do Microsoft Graph não espera reenviar a solicitação com falha.
| **unsupportedOperation**         | Não há suporte para a operação que está sendo tentada. O cliente do Microsoft Graph não espera reenviar a solicitação com falha.
| **unsupportedWorkbook**         | A solicitação falhou. A pasta de trabalho contém recursos sem suporte ou excede o limite de tamanho. O cliente do Microsoft Graph não deve reenviar a solicitação com falha até que os fatores sem suporte sejam removidos.

>**Observação:** Para o padrão normal, a solicitação com falha é definida como a solicitação correspondente à resposta. Para o padrão de operação de execução longa, a solicitação com falha é aquela que dispara a operação com falha.

### <a name="3-parse-the-top-level-error-code"></a>3. analisar o código de erro de nível superior

Se você não conseguir encontrar o código de erro de segundo nível listado no tópico [códigos de erro](/concepts/workbook-error-codes.md) , recomendamos seguir as instruções fornecidas para erros de nível superior, que estão vinculados ao código de status. Para obter detalhes sobre códigos de erro de nível superior e mensagens, consulte [códigos de erro](/concepts/workbook-error-codes.md).

### <a name="4-parse-the-status-code"></a>4. analisar o código de status

Se o código de erro que você encontrar não estiver na lista de segundo nível ou na lista de nível superior, recomendamos que você execute a ação de acordo com o código de status HTTP.

### <a name="5-error-recovery-cooldown"></a>5. recuperação de erro cooldown

Para algumas das respostas no padrão normal, uma duração de cooldown de recuperação em segundos pode ser fornecida por meio de um `Retry-After` cabeçalho. Quando uma duração de cooldown de recuperação estiver presente, o cliente do Microsoft Graph não deverá enviar solicitações de acompanhamento antes que a duração especificada seja aprovada.
<!-- {
  "type": "#page.annotation",
  "description": "Error handling in Excel Graph.",
  "keywords": "error response, error object, error codes, innerError, error handling",
  "section": "documentation",
  "tocPath": ""
} -->
