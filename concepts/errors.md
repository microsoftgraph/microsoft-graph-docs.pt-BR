---
title: Respostas de erros e tipos de recurso do Microsoft Graph
description: "  "
localization_priority: Priority
ms.openlocfilehash: cc3a0a0acacd7477c1cf686089c0235850059443
ms.sourcegitcommit: 8a74c06be9c41390331ca1717efedc5b5a244db5
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2020
ms.locfileid: "45091421"
---
# <a name="microsoft-graph-error-responses-and-resource-types"></a>Respostas de erros e tipos de recurso do Microsoft Graph

<!--In this article:
  
-   [Status code](#msg-status-code)
-   [Error resource type](#msg-error-resource-type)
-   [Code property](#msg-code-property)

<a name="msg_error_response"> </a> -->

Os erros no Microsoft Graph serão retornados por meio de códigos de status HTTP padrão, bem como um objeto de resposta de erro JSON.

## <a name="http-status-codes"></a>Códigos de status de HTTP

A tabela a seguir lista e descreve os códigos de status HTTP que podem ser retornados.

| Código de status | Mensagem de status                  | Descrição                                                                                                                            |
|:------------|:--------------------------------|:---------------------------------------------------------------------------------------------------------------------------------------|
| 400         | Solicitação Incorreta (Bad Request)                     | Não é possível processar a solicitação porque está incorreta ou mal feita.                                                                       |
| 401         | Não Autorizado (Unauthorized)                    | As informações de autenticação necessárias estão ausentes ou não são válidas para o recurso.                                                   |
| 403         | Proibido                       | Access is denied to the requested resource. The user might not have enough permission. <br /><br /> **Importante:** Se as políticas de acesso condicional forem aplicadas a um recurso, HTTP 403; Erro proibido=insufficent_claims poderá ser retornado. Para obter mais detalhes sobre o Microsoft Graph e acesso condicional confira [Diretrizes de desenvolvedor para acesso condicional do Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/active-directory-conditional-access-developer)  |
| 404         | Não Encontrado (Not Found)                       | O recurso solicitado não existe.                                                                                                  |
| 405         | Método Não Permitido (Method Not Allowed)              | O método HTTP na solicitação não é permitido no recurso.                                                                         |
| 406         | Não Aceitável (Not Acceptable)                  | Esse serviço não dá suporte ao formato solicitado no cabeçalho Accept.                                                                |
| 409         | Conflito                        | The current state conflicts with what the request expects. For example, the specified parent folder might not exist.                   |
| 410         | Sumiu (Gone)                            | O recurso solicitado não está mais disponível no servidor.                                               |
| 411         | Comprimento Solicitado (Length Required)                 | É necessário um cabeçalho Content-Length na solicitação.                                                                                    |
| 412         | Falha na Pré-condição (Precondition Failed)             | Uma pré-condição fornecida na solicitação (como um cabeçalho if-match) não corresponde ao estado atual do recurso.                       |
| 413         | Entidade de Solicitação Muito Grande (Request Entity Too Large)        | O tamanho da solicitação excede o limite máximo.                                                                                            |
| 415         | Tipo de Mídia Não Suportado (Unsupported Media Type)          | O tipo de conteúdo da solicitação é um formato sem suporte pelo serviço.                                                      |
| 416         | Intervalo Solicitado Não Satisfatório (Requested Range Not Satisfiable) | O intervalo de bytes especificado é inválido ou está indisponível.                                                                                    |
| 422         | Entidade Não Processável (Unprocessable Entity)            | Não é possível processar a solicitação porque ela está semanticamente incorreta.                                                                        |
| 423         | Bloqueado                          | O recurso acessado está bloqueado.                                                                                          |
| 429         | Muitos Pedidos (Too Many Requests)               | O aplicativo cliente foi restringido e não deve tentar repetir a solicitação antes de determinado intervalo de tempo.                |
| 500         | Erro Interno do Servidor (Internal Server Error)           | Ocorreu um erro interno do servidor ao processar a solicitação.                                                                       |
| 501         | Não Implementado (Not Implemented)                 | O recurso solicitado não foi implementado.                                                                                               |
| 503         | Serviço Indisponível (Service Unavailable)             | The service is temporarily unavailable for maintenance or is overloaded. You may repeat the request after a delay, the length of which may be specified in a Retry-After header.|
| 504         | Tempo Limite do Gateway (Gateway Timeout)                 | The server, while acting as a proxy, did not receive a timely response from the upstream server it needed to access in attempting to complete the request. May occur together with 503. |
| 507         | Armazenamento Insuficiente (Insufficient Storage)            | A cota máxima de armazenamento foi atingida.                                                                                            |
| 509         | Limite de Largura de Banda Excedido (Bandwidth Limit Exceeded)        | Your app has been throttled for exceeding the maximum bandwidth cap. Your app can retry the request again after more time has elapsed. |

The error response is a single JSON object that contains a single property named **error**. This object includes all the details of the error. You can use the information returned here instead of or in addition to the HTTP status code. The following is an example of a full JSON error body.

<!-- { "blockType": "ignored", "@odata.type": "odata.error", "expectError": true, "name": "example-error-response" } -->
```json
{
  "error": {
    "code": "invalidRange",
    "message": "Uploaded fragment overlaps with existing data.",
    "innerError": {
      "requestId": "request-id",
      "date": "date-time"
    }
  }
}
```

<!--<a name="msg_error_resource_type"> </a> -->

## <a name="error-resource-type"></a>Tipo de recurso de erro

O recurso de erro será retornado sempre que ocorrer um erro no processamento de uma solicitação.

Respostas de erro seguem a definição na especificação [OData v4](https://docs.oasis-open.org/odata/odata-json-format/v4.0/os/odata-json-format-v4.0-os.html#_Toc372793091) para respostas de erro.

### <a name="json-representation"></a>Representação JSON

O recurso de erro é composto por estes recursos:

<!-- { "blockType": "resource", "@odata.type": "odata.error" } -->
```json
{
  "error": { "@odata.type": "odata.error" }  
}
```

#### <a name="odataerror-resource-type"></a>Tipo de recurso odata.error

Dentro da resposta de erro há um recurso de erro que inclui as seguintes propriedades:

<!-- { "blockType": "resource", "@odata.type": "odata.error", "optionalProperties": [ "target", "details", "innererror"] } -->
```json
{
  "code": "string",
  "message": "string",
  "innererror": { "@odata.type": "odata.error" }
}
```

| Nome da propriedade  | Valor                  | Descrição\                                                                                               |
|:---------------|:-----------------------|:-----------------------------------------------------------------------------------------------------------|
| **code**       | string                 | Uma cadeia de códigos de erro para a falha que ocorreu                                                            |
| **message**    | string                 | A developer ready message about the error that occurred. This should not be displayed to the user directly. |
| **innererror** | error object           | Optional. Additional error objects that may be more specific than the top level error.                     |

<!--<a name="msg_code_property"> </a> -->

#### <a name="code-property"></a>Propriedade de código

The `code` property contains one of the following possible values. Your apps should be prepared to handle any one of these errors.

| Código                      | Descrição
|:--------------------------|:--------------
| **accessDenied**          | O chamador não tem permissão para executar a ação. 
| **activityLimitReached**  | O aplicativo ou o usuário foi restringido.
| **generalException**      | Ocorreu um erro não especificado.
| **invalidRange**          | O intervalo de bytes especificado é inválido ou está indisponível.
| **invalidRequest**        | A solicitação está incorreta ou foi mal formada.
| **itemNotFound**          | Não foi possível localizar o recurso.
| **malwareDetected**       | Malware detectado no recurso solicitado.
| **nameAlreadyExists**     | O nome do item especificado já existe.
| **notAllowed**            | A ação não é permitida pelo sistema.
| **notSupported**          | A solicitação não tem suporte do sistema.
| **resourceModified**      | O recurso em atualização foi alterado desde que o chamador o leu pela última vez, geralmente uma incompatibilidade de eTag.
| **resyncRequired**        | O token delta não é mais válido e o aplicativo deve redefinir o estado de sincronização.
| **serviceNotAvailable**   | The service is not available. Try the request again after a delay. There may be a Retry-After header. 
| **syncStateNotFound**     | As gerações do estado de sincronização não foram encontradas. O token delta está expirado e os dados precisam ser novamente sincronizados. 
| **quotaLimitReached**     | O usuário atingiu seu limite de cota.
| **unauthenticated**       | O chamador não está autenticado.

The `innererror` object might recursively contain more `innererror` objects with additional, more specific error codes. When handling an error, apps should loop through all the error codes available and use the most detailed one that they understand. Some of the more detailed codes are listed at the bottom of this page.

To verify that an error object is an error you are expecting, you must loop over the `innererror` objects, looking for the error codes you expect. For example:

```csharp
public bool IsError(string expectedErrorCode)
{
    OneDriveInnerError errorCode = this.Error;
    while (null != errorCode)
    {
        if (errorCode.Code == expectedErrorCode)
            return true;
        errorCode = errorCode.InnerError;
    }
    return false;
}
```

Para um exemplo que mostra como lidar de maneira apropriada com erros, consulte [Tratamento de Código de Erro](https://gist.github.com/rgregg/a1866be15e685983b441).

The `message` property at the root contains an error message intended for the developer to read. Error messages are not localized and shouldn't be displayed directly to the user. When handling errors, your code should not key off of `message` values because they can change at any time, and they often contain dynamic information specific to the failed request. You should only code against error codes returned in `code` properties.

#### <a name="detailed-error-codes"></a>Códigos de erro detalhados
The following are some additional errors that your app might encounter within the nested `innererror` objects. Apps are not required to handle these, but can if they choose. The service might add new error codes or stop returning old ones at any time, so it is important that all apps be able to handle the [basic error codes](#code-property).

| Código                               | Descrição
|:-----------------------------------|:----------------------------------------------------------
| **accessRestricted**               | Acesso restrito ao proprietário do item.
| **cannotSnapshotTree**             | Failed to get a consistent delta snapshot. Try again later.
| **childItemCountExceeded**         | Limite máximo do número de itens filhos atingido.
| **entityTagDoesNotMatch**          | ETag não corresponde ao valor do item atual.
| **fragmentLengthMismatch**         | O tamanho total declarado para esse fragmento é diferente do da sessão de carregamento.
| **fragmentOutOfOrder**             | O fragmento carregado está fora da ordem.
| **fragmentOverlap**                | Fragmento carregado sobrepõe-se a dados existentes.
| **invalidAcceptType**              | Tipo de aceitação inválido.
| **invalidParameterFormat**         | Formato de parâmetro inválido.
| **invalidPath**                    | O nome contém caracteres inválidos.
| **invalidQueryOption**             | Opção de consulta inválida.
| **invalidStartIndex**              | Índice de início inválido.
| **lockMismatch**                   | O token de bloqueio não corresponde ao bloqueio existente.
| **lockNotFoundOrAlreadyExpired**   | Não há atualmente nenhum bloqueio expirado no item.
| **lockOwnerMismatch**              | A ID do proprietário do bloqueio não corresponde à ID fornecida.
| **malformedEntityTag**             | ETag header is malformed. ETags must be quoted strings.
| **maxDocumentCountExceeded**       | Atingido o limite máximo do número de documentos.
| **maxFileSizeExceeded**            | Tamanho máximo do arquivo excedido.
| **maxFolderCountExceeded**         | Atingido o limite máximo do número de pastas.
| **maxFragmentLengthExceeded**      | Tamanho máximo do arquivo excedido.
| **maxItemCountExceeded**           | Limite máximo do número de itens atingido.
| **maxQueryLengthExceeded**         | Comprimento máximo de consulta excedido.
| **maxStreamSizeExceeded**          | Tamanho máximo de fluxo excedido.
| **parameterIsTooLong**             | Parâmetro excede o comprimento máximo.
| **parameterIsTooSmall**            | Parâmetro é menor que o valor mínimo.
| **pathIsTooLong**                  | O caminho excede o comprimento máximo.
| **pathTooDeep**                    | Atingido o limite de profundidade da hierarquia de pastas.
| **propertyNotUpdateable**          | Propriedade não atualizável.
| **resyncApplyDifferences**         | Resync required. Replace any local items with the server's version (including deletes) if you're sure that the service was up to date with your local changes when you last sync'd. Upload any local changes that the server doesn't know about.
| **resyncRequired**                 | Nova sincronização é necessária.
| **resyncUploadDifferences**        | Resync required. Upload any local items that the service did not return, and upload any files that differ from the server's version (keeping both copies if you're not sure which one is more up-to-date).
| **serviceNotAvailable**            | O servidor não consegue processar a solicitação atual.
| **serviceReadOnly**                | O recurso é temporariamente somente leitura.
| **throttledRequest**               | Muitos pedidos.
| **tooManyResultsRequested**        | Muitos resultados solicitados.
| **tooManyTermsInQuery**            | Muitos termos na consulta.
| **totalAffectedItemCountExceeded** | Operação não permitida porque o número de itens afetados excede o limite.
| **truncationNotAllowed**           | O truncamento de dados não é permitido.
| **uploadSessionFailed**            | Falha na sessão de carregamento.
| **uploadSessionIncomplete**        | Sessão de carregamento incompleta.
| **uploadSessionNotFound**          | Sessão de carregamento não encontrada.
| **virusSuspicious**                | Este documento é suspeito e pode conter um vírus.
| **zeroOrFewerResultsRequested**    | Nenhum ou poucos resultados solicitados.


<!-- {
  "type": "#page.annotation",
  "description": "Understand the error format for the API and error codes.",
  "keywords": "error response, error, error codes, innererror, message, code",
  "section": "documentation",
  "suppressions": [
    " Warning: /concepts/errors.md:
      Multiple resources found in file, but we only support one per file. 'odata.error,odata.error'. Skipping."
  ],
  "tocPath": "Misc/Error Responses"
} -->
