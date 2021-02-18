---
title: Tratamento de erros para APIs do Excel no Microsoft Graph
description: Instruções de tratamento de erros para APIs do Excel no Microsoft Graph
author: grangeryy
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 5d5a420b4968b0a944ac192de5654692678663c8
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/18/2021
ms.locfileid: "50293075"
---
# <a name="error-handling-for-excel-apis-in-microsoft-graph"></a>Tratamento de erros para APIs do Excel no Microsoft Graph

Este artigo fornece instruções gerais e sugestões para lidar com erros retornados pelas APIs do Excel no Microsoft Graph quando uma solicitação enviada por meio da API falha.

## <a name="types-of-error-responses"></a>Tipos de respostas de erro

As APIs do Excel no Microsoft Graph retornam dois tipos de erros. Uma é a resposta de erro regular, que se parece com o seguinte.

```http
HTTP/1.1 <HTTP status code>
Content-type: application/json

{
  "error": <Error object>
}
```

O segundo é do padrão de operação de longa execução, que pode retornar um código de status HTTP e o status da operação no corpo da resposta, como `200 OK` no exemplo a `failed` seguir.

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "status": "failed",
  "error": <Error object>
}
```

Para ambas as respostas de erro, o objeto de erro tem a seguinte estrutura.

>**Observação:** As respostas de erro seguem a definição na [especificação OData v4](https://docs.oasis-open.org/odata/odata-json-format/v4.0/os/odata-json-format-v4.0-os.html#_Toc372793091) para respostas de erro.

```json
{
  "code": "string",
  "message": "string",
  "innerError": { "@odata.type": "odata.error" }
}
```

O objeto `innerError` pode conter repetidamente mais objetos `innerError` com códigos de erro adicionais, mais específicos. Por exemplo, o objeto de erro pode conter informações de erro mais detalhadas no código de erro de segundo nível e na mensagem, conforme mostrado.

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

Os clientes do Microsoft Graph podem usar as etapas a seguir para lidar com erros que ocorrem com as APIs do Excel.

### <a name="1-determine-whether-it-is-a-long-running-operation-error"></a>1. Determinar se é um erro de operação de longa execução

Antes de manipular um erro, a primeira etapa é determinar se a resposta de erro é de um padrão de operação de longa execução ou de um padrão regular. Um erro de operação de execução longa retornará um código de status HTTP e o status da operação `200 OK` `failed` no corpo da resposta. Uma resposta de erro regular retornará um código de status de erro HTTP correspondente. 

### <a name="2-parse-second-level-error-code"></a>2. Analisar o código de erro de segundo nível

Para o padrão de operação de longa execução e o padrão regular, recomendamos que você siga primeiro as instruções para erros de segundo nível. O código de erro não faz parte de maiúsculas e minúsculas. A tabela a seguir lista as instruções para alguns dos erros. O serviço pode adicionar novos códigos de erro a qualquer momento.

| Código                               | Instruções
|:-----------------------------------|:---------------------------------------------
| **accessConflict**   | A solicitação com falha está em conflito com outros clientes que acessam a área de trabalho (por exemplo, outro cliente tloquei a agenda para edição). Não se espera que o cliente do Microsoft Graph reende a solicitação com falha até que o conflito seja resolvido. Um usuário final pode optar por executar manualmente as mesmas operações com o Excel Online para obter mais detalhes sobre o conflito.
| **accessDenied**   | Não é possível executar a operação solicitada (por exemplo, realizar alterações em células bloqueadas). Não se espera que o cliente do Microsoft Graph reende a solicitação com falha.
| **badRequestUncategorized**    | Um erro não especificado é encontrado na solicitação com falha. Não se espera que o cliente do Microsoft Graph reende a solicitação com falha.
| **conflictUncategorized**                   | A solicitação com falha está em conflito com determinado estado do servidor. Não se espera que o cliente do Microsoft Graph reende a solicitação com falha até que o conflito seja resolvido. Um usuário final pode optar por executar manualmente as mesmas operações com o Excel Online para obter mais detalhes sobre o conflito.
| **filteredRangeConflict**                   | A operação falhou porque está em conflito com um intervalo filtrado. Não se espera que o cliente do Microsoft Graph reende a solicitação com falha.
| **forbiddenUncategorized**                    | A solicitação com falha não é permitida. Não se espera que o cliente do Microsoft Graph reende a solicitação com falha. Um usuário final pode optar por executar manualmente as mesmas operações com o Excel Online para obter mais detalhes sobre as restrições.
| **gatewayTimeoutUncategorized**         | O serviço não pôde concluir a solicitação dentro do limite de tempo.
| **generalException**         | Ocorreu um erro interno durante o processamento da solicitação. Não se espera que o cliente do Microsoft Graph reende a solicitação com falha.
| **insertDeleteConflict**         | A tentativa de operação de exclusão ou inserção resultou em um conflito. Não se espera que o cliente do Microsoft Graph reende a solicitação com falha.
| **internalServerErrorUncategorized**       | Ocorreu um erro não especificado. Não se espera que o cliente do Microsoft Graph reende a solicitação com falha. Se uma sessão for especificada na solicitação com falha, o acesso à sessão também não será esperado.
| **invalidArgument**         | O argumento é inválido, está ausente ou tem um formato incorreto. Não se espera que o cliente do Microsoft Graph reende a solicitação com falha.
| **invalidReference**         | Esta referência não é válida para a operação atual. Não se espera que o cliente do Microsoft Graph reende a solicitação com falha.
| **invalidSessionAccessConflict**             | A sessão especificada na solicitação é inválida devido a conflitos com outros clientes que estão acessando a área de trabalho (por exemplo, outro cliente tiver bloqueado a agenda para edição). Não se espera mais acesso à sessão especificada na solicitação com falha. A recriação de sessões com a mesma **solicitação createSession** não é esperada até que o conflito seja resolvido. Recriar sessões com uma solicitação **createSession** diferente pode ou não ter êxito. Um usuário final pode optar por executar manualmente as mesmas operações com o Excel Online para obter mais detalhes sobre o conflito.
| **invalidSessionAuthentication**         | A sessão especificada na solicitação é inválida devido a um erro de autenticação. Não se espera mais acesso à sessão especificada na solicitação com falha. A recriação de sessões com a mesma **solicitação createSession** não é esperada até que as informações de autenticação apropriadas são fornecidas.
| **invalidSessionNotFound**         | A sessão especificada na solicitação é inválida porque a agenda não foi encontrada. Não se espera mais acesso à sessão especificada na solicitação com falha. A recriação de sessões com a mesma **solicitação createSession** não é esperada.
| **invalidSessionReCreatable**             | A sessão especificada na solicitação não existe ou é inválida devido a um erro transitório. O cliente do Microsoft Graph pode tentar recriar uma sessão e retomar o trabalho. Não se espera mais acesso à sessão especificada na solicitação com falha.
| **invalidSessionRestricted**          | A sessão especificada na solicitação é inválida devido a restrições ou configurações de serviço. Não se espera mais acesso à sessão especificada na solicitação com falha. A recriação de sessões com a mesma **solicitação createSession** não é esperada até que as restrições ou configurações que bloqueiam a solicitação mudem. Recriar sessões com uma solicitação **createSession** diferente pode ou não ter êxito. Um usuário final pode optar por executar manualmente as mesmas operações com o Excel Online para obter mais detalhes das restrições.
| **invalidSessionUnexpected**                | A sessão especificada na solicitação é inválida devido a um problema inesperado. Não se espera mais acesso à sessão especificada na solicitação com falha. A recriação de sessões com a mesma **solicitação createSession** não é esperada. Recriar sessões com uma solicitação **createSession** diferente pode ou não ter êxito.
| **invalidSessionUnsupportedWorkbook**              | A sessão especificada na solicitação é inválida porque a área de trabalho contém recursos sem suporte ou excede o limite de tamanho. Geralmente, os fatores sem suporte são introduzidos por outro cliente que acessa a agenda. Não se espera mais acesso à sessão especificada na solicitação com falha. A recriação de sessões com a mesma **solicitação createSession** não é esperada até que os fatores sem suporte sejam removidos. Recriar sessões com uma solicitação createSession diferente pode ou não ter êxito. Um usuário final pode optar por executar manualmente as mesmas operações com o Excel Online para obter mais detalhes dos fatores sem suporte ou com a Área de Trabalho do Excel onde a planilha pode ter suporte.
| **itemAlreadyExists**         | O recurso que está sendo criado já existe. Não se espera que o cliente do Microsoft Graph reende a solicitação com falha.
| **itemNotFound**         | O recurso solicitado não existe. Não se espera que o cliente do Microsoft Graph reende a solicitação com falha.
| **methodNotAllowed**         | O método HTTP especificado na solicitação não é permitido no recurso. Não se espera que o cliente do Microsoft Graph reende a solicitação com falha.
| **methodNotAllowedUncategorized**              | O método HTTP especificado na solicitação não é permitido no recurso. Não se espera que o cliente do Microsoft Graph reende a solicitação com falha.
| **nonBlankCellOffSheet**         | Não é possível inserir novas células porque ela tiraria as células não vazias do final da planilha. Não se espera que o cliente do Microsoft Graph reende a solicitação com falha.
| **notFoundUncategorized**             | O recurso solicitado não pode ser encontrado. Não se espera que o cliente do Microsoft Graph reende a solicitação com falha.
| **notImplementedUncategorized**            | O recurso solicitado não está implementado no momento. Não se espera que o cliente do Microsoft Graph reende a solicitação com falha.
| **payloadTooLargeUncategorized**              | A carga da solicitação excede o limite de tamanho. Não se espera que o cliente do Microsoft Graph reende a solicitação com falha.
| **rangeExceedsLimit**         | A contagem de células no intervalo excedeu o número máximo suportado. O cliente do Microsoft Graph pode tentar enviar uma solicitação com um tamanho de intervalo menor.
| **requestAborted**         | A solicitação foi anulada durante o tempo de executar, o que geralmente foi causado por um cálculo de tempo longo de funções na agenda. Não se espera que o cliente do Microsoft Graph reende a solicitação com falha.
| **serviceUnavailableUncategorized**      | O serviço está temporariamente indisponível ou sobrecarregado. Não se espera que o cliente do Microsoft Graph reende a solicitação com falha até que a duração da recarga especificada passe.
| **tooManyRequestsUncategorized**             | A solicitação com falha excede determinada limitação de frequência. Não se espera que o cliente do Microsoft Graph reende a solicitação com falha até que a duração da recarga especificada passe.
| **transientFailure**           | A solicitação falhou devido a um erro transitório. Não se espera que o cliente do Microsoft Graph reende a solicitação com falha até que a duração da recarga especificada passe.
| **unauthorizedUncategorized**         | As informações de autenticação necessárias para o recurso estão ausentes ou são inválidas. Não se espera que o cliente do Microsoft Graph reende a solicitação com falha.
| **unsupportedOperation**         | Não há suporte para a operação que está sendo tentada. Não se espera que o cliente do Microsoft Graph reende a solicitação com falha.
| **unsupportedWorkbook**         | A solicitação falhou. A área de trabalho contém recursos sem suporte ou excede o limite de tamanho. Não se espera que o cliente do Microsoft Graph reende a solicitação com falha até que os fatores sem suporte sejam removidos.

>**Observação:** Para o padrão regular, a solicitação com falha é definida como a solicitação correspondente à resposta. Para o padrão de operação de longa execução, a solicitação com falha é a que dispara a operação com falha.

### <a name="3-parse-the-top-level-error-code"></a>3. Analisar o código de erro de nível superior

Se você não encontrar o código de erro [](workbook-error-codes.md#detailed-error-code) de segundo nível listado no tópico Códigos de erro detalhados, recomendamos seguir as instruções fornecidas para erros de nível superior. Os códigos de erro de nível superior são vinculados ao código de status e você pode agir de acordo com os códigos de status correspondentes. Para obter detalhes sobre códigos de erro de nível superior e mensagens, consulte [Códigos de erro.](workbook-error-codes.md#error-code)

### <a name="4-parse-the-status-code"></a>4. Analisar o código de status

Se o código de erro encontrado não estiver na lista de segundo nível ou na lista de nível superior, recomendamos que você tome medidas de acordo com o código de status HTTP.

### <a name="5-error-recovery-cooldown"></a>5. Rebaixamento de recuperação de erros

Para algumas das respostas no padrão regular, uma duração de rebaixamento de recuperação em segundos pode ser fornecida por meio de `Retry-After` um header. Quando uma duração de rebaixamento de recuperação está presente, não se espera que o cliente do Microsoft Graph envie solicitações de acompanhamento antes que a duração especificada passe.

## <a name="special-case-handling"></a>Tratamento de caso especial

Para [](excel-manage-sessions.md#request-types)solicitações de sessão , se você encontrar um ou erro, quando um código de erro de segundo nível é listado em códigos de erro detalhados , analisar o código de segundo nível e seguir as instruções correspondentes; caso contrário, reenviamos que você recriar a sessão `502/badGateway` `503/serviceUnavailable` diretamente. [](workbook-error-codes.md#detailed-error-code)
<!-- {
  "type": "#page.annotation",
  "description": "Error handling in Excel Graph.",
  "keywords": "error response, error object, error codes, innerError, error handling",
  "section": "documentation",
  "tocPath": ""
} -->
