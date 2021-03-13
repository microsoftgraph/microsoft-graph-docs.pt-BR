---
title: Respostas de erros e tipos de recurso do Microsoft Graph
description: Este tópico descreve alguns dos erros que podem ser retornados nas respostas do Microsoft Graph.
localization_priority: Priority
ms.openlocfilehash: a893f7e06d89bf50cbcc4cc13a1e394b6da2d72a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50777009"
---
# <a name="microsoft-graph-error-responses-and-resource-types"></a>Respostas de erros e tipos de recurso do Microsoft Graph

Os erros no Microsoft Graph serão retornados por meio de códigos de status HTTP padrão, bem como um objeto de resposta de erro JSON.

## <a name="http-status-codes"></a>Códigos de status de HTTP

A tabela a seguir lista e descreve os códigos de status HTTP que podem ser retornados.

| Código de status | Mensagem de status                  | Descrição                                                                                                                            |
|:------------|:--------------------------------|:---------------------------------------------------------------------------------------------------------------------------------------|
| 400         | Solicitação Incorreta (Bad Request)                     | Não é possível processar a solicitação porque está incorreta ou mal feita.                                                                       |
| 401         | Não Autorizado (Unauthorized)                    | As informações de autenticação necessárias estão ausentes ou não são válidas para o recurso.                                                   |
| 403         | Proibido                       | Acesso negado ao recurso solicitado. O usuário pode não ter permissão suficiente. <br /><br /> **Importante:** Se as políticas de acesso condicional forem aplicadas a um recurso, HTTP 403; Erro proibido=insufficent_claims poderá ser retornado. Para obter mais detalhes sobre o Microsoft Graph e acesso condicional confira [Diretrizes de desenvolvedor para acesso condicional do Azure Active Directory](/azure/active-directory/develop/active-directory-conditional-access-developer)  |
| 404         | Não Encontrado (Not Found)                       | O recurso solicitado não existe.                                                                                                  |
| 405         | Método Não Permitido (Method Not Allowed)              | O método HTTP na solicitação não é permitido no recurso.                                                                         |
| 406         | Não Aceitável (Not Acceptable)                  | Esse serviço não dá suporte ao formato solicitado no cabeçalho Accept.                                                                |
| 409         | Conflito                        | O estado atual está em conflito com o que a solicitação espera. Por exemplo, a pasta pai especificada não existe.                   |
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
| 503         | Serviço Indisponível (Service Unavailable)             | O serviço está temporariamente indisponível para manutenção ou está sobrecarregado. Você pode repetir a solicitação após um atraso, cujo comprimento pode ser especificado em um cabeçalho Retry-After.|
| 504         | Tempo Limite do Gateway (Gateway Timeout)                 | O servidor, ao atuar como um proxy, não recebeu uma resposta em tempo hábil do servidor upstream necessário para acessar a tentativa de concluir a solicitação. Pode ocorrer com 503. |
| 507         | Armazenamento Insuficiente (Insufficient Storage)            | A cota máxima de armazenamento foi atingida.                                                                                            |
| 509         | Limite de Largura de Banda Excedido (Bandwidth Limit Exceeded)        | Seu aplicativo foi limitado por exceder o limite máximo de largura de banda. O aplicativo pode tentar a solicitação novamente depois de decorrido algum tempo. |

A resposta de erro é um único objeto JSON que contém uma propriedade única chamada **error**. Esse objeto inclui todos os detalhes do erro. Você pode usar as informações retornadas aqui em vez de ou além do código de status HTTP. Este é um exemplo de um corpo de erro JSON completo.

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

| Nome da propriedade  | Valor                  | Descrição                                                                                                |
|:---------------|:-----------------------|:-----------------------------------------------------------------------------------------------------------|
| **code**       | string                 | Uma cadeia de códigos de erro para a falha que ocorreu                                                            |
| **message**    | string                 | Uma mensagem pronta do programador sobre o erro que ocorreu. Esta não deve ser apresentada diretamente ao usuário. |
| **innererror** | error object           | Opcional. Objetos error adicionais que podem ser mais específicos do que o erro de nível superior.                     |

<!--<a name="msg_code_property"> </a> -->

#### <a name="code-property"></a>Propriedade de código

A propriedade `code` contém um dos valores possíveis a seguir. Seus aplicativos devem estar preparados para lidar com qualquer um destes erros.

| Código                      | Descrição
|:--------------------------|:--------------
| **accessDenied**          | O chamador não tem permissão para executar a ação. 
| **activityLimitReached**  | O aplicativo ou o usuário foi restringido.
| **extensionError**        | A caixa de correio está localizada no local e o servidor do Exchange não dá suporte a solicitações federadas do Microsoft Graph, ou uma [política de aplicativo](./auth-limit-mailbox-access.md) impede que o aplicativo acesse a caixa de correio.
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
| **serviceNotAvailable**   | O serviço não está disponível. Tente fazer a solicitação novamente após um atraso. Pode haver um cabeçalho Retry-After 
| **syncStateNotFound**     | As gerações do estado de sincronização não foram encontradas. O token delta está expirado e os dados precisam ser novamente sincronizados. 
| **quotaLimitReached**     | O usuário atingiu seu limite de cota.
| **unauthenticated**       | O chamador não está autenticado.

O objeto `innererror` pode conter repetidamente mais objetos `innererror` com códigos de erro adicionais, mais específicos. Ao lidar com um erro, os aplicativos devem percorrer todos os códigos de erro disponíveis e usar o mais detalhado que consigam entender. Alguns dos códigos mais detalhados estão listados na parte inferior desta página.

Para verificar se um objeto de erro é um erro que você está esperando, execute um loop sobre os objetos `innererror` procurando os códigos de erro que você espera. Por exemplo:

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

A propriedade `message` na raiz contém uma mensagem de erro destinada ao desenvolvedor. As mensagens de erro não são localizadas e não devem ser exibidas diretamente para o usuário. Ao tratar de erros, seu código não deve desviar dos valores `message` porque eles podem mudar a qualquer momento e geralmente contêm informações dinâmicas específicas para a solicitação com falha. Você só deve escrever códigos contra códigos de erro retornados nas propriedades `code`.

#### <a name="detailed-error-codes"></a>Códigos de erro detalhados
A seguir estão alguns erros adicionais que seu aplicativo pode encontrar nos objetos aninhados `innererror`. Os aplicativos não são obrigados a tratar deles, mas podem, se quiserem. O serviço pode adicionar novos códigos de erro ou parar de retornar os antigos a qualquer hora; portanto, é importante que todos os aplicativos consigam tratar dos [códigos de erro básicos](#code-property).

| Código                               | Descrição
|:-----------------------------------|:----------------------------------------------------------
| **accessRestricted**               | Acesso restrito ao proprietário do item.
| **cannotSnapshotTree**             | Falha ao obter um instantâneo delta consistente. Tente novamente mais tarde.
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
| **malformedEntityTag**             | O Cabeçalho ETag está mal feito. ETags devem ser cadeias de caracteres entre aspas.
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
| **resyncApplyDifferences**         | Nova sincronização necessária. Substitua todos os itens locais com a versão do servidor (incluindo exclusões) se você tiver certeza de que o serviço estava atualizado com suas alterações locais quando você sincronizou pela última vez. Carregar alterações locais que o servidor não conhece.
| **resyncRequired**                 | Nova sincronização é necessária.
| **resyncUploadDifferences**        | Nova sincronização necessária. Carregue os itens locais que o serviço não retornou e carregue os arquivos que diferem da versão do servidor (mantendo ambas as cópias se você não tiver certeza de qual é a mais atual).
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
