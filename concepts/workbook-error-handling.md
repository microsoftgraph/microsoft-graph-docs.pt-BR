---
title: Tratamento de erros para APIs do Excel
description: Encontre instruções gerais e sugestões para lidar com erros retornados pelas APIs do Excel no Microsoft Graph quando uma solicitação enviada por meio da API falhar.
author: grangeryy
ms.localizationpriority: medium
ms.prod: excel
ms.openlocfilehash: 7e115fe0a09c519ecad98f49524ca3ebd86001fd
ms.sourcegitcommit: cf2b3c67cb9ce832944cfbac66171590bbbd83de
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/06/2022
ms.locfileid: "66645413"
---
# <a name="error-handling-for-excel-apis"></a>Tratamento de erros para APIs do Excel

Este artigo fornece instruções gerais e sugestões para lidar com erros retornados pelas [APIs do Excel](/graph/api/resources/excel) no Microsoft Graph quando uma solicitação enviada por meio da API falha.

## <a name="types-of-error-responses"></a>Tipos de respostas de erro

As APIs do Excel no Microsoft Graph retornam dois tipos de erros. Uma delas é a resposta de erro regular, que se parece com a seguinte.

```http
HTTP/1.1 <HTTP status code>
Content-type: application/json
Retry-After: <Cooldown duration in seconds> (optional)

{
  "error": <Error object>
}
```

O segundo é do padrão de operação de execução longa, `200 OK` que pode retornar um código de status `failed` HTTP e o status da operação no corpo da resposta, como no exemplo a seguir.

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "status": "failed",
  "error": <Error object>
}
```

Para ambas as respostas de erro, o objeto de erro tem a estrutura a seguir.

> [!NOTE]
> Respostas de erro seguem a definição na especificação [OData v4](https://docs.oasis-open.org/odata/odata-json-format/v4.0/os/odata-json-format-v4.0-os.html#_Toc372793091) para respostas de erro.

```json
{
  "code": "string",
  "message": "string",
  "innerError": { "@odata.type": "odata.error" }
}
```

O **objeto innerError** pode conter recursivamente mais **objetos innerError** com códigos de erro adicionais e mais específicos. Por exemplo, o objeto de erro pode conter informações de erro mais detalhadas no código de erro de segundo nível e na mensagem, conforme mostrado.

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

Espera-se que os clientes do Microsoft Graph usem as etapas a seguir para lidar com erros que ocorrem com APIs do Excel.

### <a name="1-determine-whether-it-is-a-long-running-operation-error"></a>1. Determinar se é um erro de operação de execução longa

Antes de tratar um erro, a primeira etapa é determinar se a resposta de erro é de um padrão de operação de execução longa ou um padrão regular. Um erro de operação de execução longa retornará um código `200 OK` de status `failed` HTTP e o status da operação no corpo da resposta. Uma resposta de erro regular retornará um código de status de erro HTTP correspondente. 

### <a name="2-parse-second-level-error-code"></a>2. Analisar código de erro de segundo nível

Para o padrão de operação de execução longa e o padrão regular, o cliente deve primeiro analisar os códigos de erro de segundo nível necessários e manipulá-los de acordo com as instruções. Opcionalmente, o cliente também pode lidar com outros códigos de erro de segundo nível ou optar por fazer fallback para códigos de erro de nível superior [ou](#3-parse-the-top-level-error-code) [códigos de status](#4-parse-the-status-code).

Os códigos de erro não diferenciam maiúsculas de minúsculas.

#### <a name="required-second-level-error-codes"></a>Códigos de erro de segundo nível necessários

A tabela a seguir lista as instruções para os códigos de erro de segundo nível necessários que os clientes do Microsoft Graph devem manipular. O serviço pode adicionar novos códigos de erro a qualquer momento.

| Código                               | Instruções
|:-----------------------------------|:---------------------------------------------
| `accessConflict`   | A solicitação com falha entra em conflito com outros clientes que acessam a pasta de trabalho (por exemplo, outro cliente trancou a pasta de trabalho para edição). O cliente do Microsoft Graph não deve reenviar a solicitação com falha até que o conflito seja resolvido. Um usuário final pode optar por executar manualmente as mesmas operações com o Excel Online para obter mais detalhes sobre o conflito.
| `badRequestUncategorized`    | Um erro não especificado é encontrado na solicitação com falha. Não é esperado que o cliente do Microsoft Graph reenvie a solicitação com falha.
| `conflictUncategorized`                   | A solicitação com falha entra em conflito com determinado estado do servidor. O cliente do Microsoft Graph não deve reenviar a solicitação com falha até que o conflito seja resolvido. Um usuário final pode optar por executar manualmente as mesmas operações com o Excel Online para obter mais detalhes sobre o conflito.
| `forbiddenUncategorized`                    | A solicitação com falha não é permitida. Não é esperado que o cliente do Microsoft Graph reenvie a solicitação com falha. Um usuário final pode optar por executar manualmente as mesmas operações com o Excel Online para obter mais detalhes sobre as restrições.
| `gatewayTimeoutUncategorized`         | O serviço não pôde concluir a solicitação dentro do limite de tempo.
| `internalServerErrorUncategorized`       | Ocorreu um erro não especificado. Não é esperado que o cliente do Microsoft Graph reenvie a solicitação com falha. Se uma sessão for especificada na solicitação com falha, o acesso adicional à sessão também não será esperado.
| `invalidSessionAccessConflict`             | A sessão especificada na solicitação é inválida devido a conflitos com outros clientes que estão acessando a pasta de trabalho (por exemplo, outro cliente trancou a pasta de trabalho para edição). Não é esperado acesso adicional à sessão especificada na solicitação com falha. A recriação de sessões com a mesma **solicitação createSession** não é esperada até que o conflito seja resolvido. Recriar sessões com uma solicitação **createSession** diferente pode ou não ser bem-sucedida. Um usuário final pode optar por executar manualmente as mesmas operações com o Excel Online para obter mais detalhes sobre o conflito.
| `invalidSessionAuthentication`         | A sessão especificada na solicitação é inválida devido a um erro de autenticação. Não é esperado acesso adicional à sessão especificada na solicitação com falha. A recriação de sessões com a mesma **solicitação createSession** não é esperada até que as informações de autenticação apropriadas sejam fornecidas.
| `invalidSessionNotFound`         | A sessão especificada na solicitação é inválida porque a pasta de trabalho não pode ser encontrada. Não é esperado acesso adicional à sessão especificada na solicitação com falha. Não é esperado recriar sessões com a mesma **solicitação createSession** .
| `invalidSessionReCreatable`             | A sessão especificada na solicitação não existe ou é inválida devido a um erro transitório. O cliente do Microsoft Graph pode tentar recriar uma sessão e retomar o trabalho. Não é esperado acesso adicional à sessão especificada na solicitação com falha.
| `invalidSessionRestricted`          | A sessão especificada na solicitação é inválida devido a restrições ou configurações de serviço. Não é esperado acesso adicional à sessão especificada na solicitação com falha. A recriação de sessões com a mesma **solicitação createSession** não é esperada até que as restrições ou configurações que bloqueiam a solicitação sejam alteradas. Recriar sessões com uma solicitação **createSession** diferente pode ou não ser bem-sucedida. Um usuário final pode optar por executar manualmente as mesmas operações com o Excel Online para obter mais detalhes sobre as restrições.
| `invalidSessionUnexpected`                | A sessão especificada na solicitação é inválida devido a um problema inesperado. Não é esperado acesso adicional à sessão especificada na solicitação com falha. Não é esperado recriar sessões com a mesma **solicitação createSession** . Recriar sessões com uma solicitação **createSession** diferente pode ou não ser bem-sucedida.
| `invalidSessionUnsupportedWorkbook`              | A sessão especificada na solicitação é inválida porque a pasta de trabalho contém recursos sem suporte ou excede o limite de tamanho. Normalmente, os fatores sem suporte são introduzidos por outro cliente que acessa a pasta de trabalho. Não é esperado acesso adicional à sessão especificada na solicitação com falha. A recriação de sessões com a mesma **solicitação createSession** não é esperada até que os fatores sem suporte sejam removidos. Recriar sessões com uma solicitação createSession diferente pode ou não ser bem-sucedida. Um usuário final pode optar por executar manualmente as mesmas operações com o Excel Online para obter mais detalhes dos fatores sem suporte ou com a Área de Trabalho do Excel em que a pasta de trabalho pode ter suporte.
| `methodNotAllowedUncategorized`              | O método HTTP especificado na solicitação não é permitido no recurso. Não é esperado que o cliente do Microsoft Graph reenvie a solicitação com falha.
| `notFoundUncategorized`             | O recurso solicitado não pode ser encontrado. Não é esperado que o cliente do Microsoft Graph reenvie a solicitação com falha.
| `notImplementedUncategorized`            | O recurso solicitado não está implementado no momento. Não é esperado que o cliente do Microsoft Graph reenvie a solicitação com falha.
| `payloadTooLargeUncategorized`              | O conteúdo da solicitação excede o limite de tamanho. Não é esperado que o cliente do Microsoft Graph reenvie a solicitação com falha.
| `serviceUnavailableUncategorized`      | O serviço está temporariamente indisponível ou está sobrecarregado. O cliente do Microsoft Graph não deve reenviar a solicitação com falha até que a duração de resfriamento especificada passe.
| `tooManyRequestsUncategorized`             | A solicitação com falha excede determinada limitação de frequência. O cliente do Microsoft Graph não deve reenviar a solicitação com falha até que a duração de resfriamento especificada passe. Para obter as práticas recomendadas para reduzir a limitação, consulte [Reduzir erros de limitação](workbook-best-practice.md#reduce-throttling-errors).
| `transientFailure`           | A solicitação falhou devido a um erro transitório. O cliente do Microsoft Graph não deve reenviar a solicitação com falha até que a duração de resfriamento especificada passe.
| `unauthorizedUncategorized`         | As informações de autenticação necessárias para o recurso estão ausentes ou inválidas. Não é esperado que o cliente do Microsoft Graph reenvie a solicitação com falha.
| `unsupportedWorkbook`         | A solicitação falhou. A pasta de trabalho contém recursos sem suporte ou excede o limite de tamanho. O cliente do Microsoft Graph não deve reenviar a solicitação com falha até que os fatores sem suporte sejam removidos.

> [!NOTE]
> Para o padrão regular, a solicitação com falha é definida como a solicitação que corresponde à resposta. Para o padrão de operação de execução longa, a solicitação com falha é aquela que dispara a operação com falha.

#### <a name="optional-second-level-error-code-examples"></a>Exemplos opcionais de código de erro de segundo nível

A tabela a seguir lista exemplos de códigos de erro opcionais de segundo nível, incluindo as instruções de tratamento correspondentes para cada código de erro. O serviço pode adicionar novos códigos de erro a qualquer momento.

| Código                      | Instruções                                                                                                                                                                                                                                                                                                                           |
|:--------------------------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `accessDenied`          | Não é possível executar a operação solicitada (por exemplo, executar alterações em células bloqueadas). Não é esperado que o cliente do Microsoft Graph reenvie a solicitação com falha.                                                                                                                                                                 |
| `filteredRangeConflict` | A operação falhou porque está em conflito com um intervalo filtrado. Não é esperado que o cliente do Microsoft Graph reenvie a solicitação com falha.                                                                                                                                                                                              |
| `generalException`      | Ocorreu um erro interno durante o processamento da solicitação. Não é esperado que o cliente do Microsoft Graph reenvie a solicitação com falha.                                                                                                                                                                                                      |
| `insertDeleteConflict`  | A tentativa de operação de exclusão ou inserção resultou em um conflito. Não é esperado que o cliente do Microsoft Graph reenvie a solicitação com falha. Um usuário final pode optar por executar manualmente as mesmas operações com o Excel Online para obter mais detalhes sobre o conflito.                                                                     |
| `invalidArgument`       | O argumento é inválido, está ausente ou tem um formato incorreto. Não é esperado que o cliente do Microsoft Graph reenvie a solicitação com falha.                                                                                                                                                                                                |
| `invalidReference`      | Esta referência não é válida para a operação atual. Não é esperado que o cliente do Microsoft Graph reenvie a solicitação com falha.                                                                                                                                                                                                        |
| `itemAlreadyExists`     | O recurso que está sendo criado já existe. Não é esperado que o cliente do Microsoft Graph reenvie a solicitação com falha.                                                                                                                                                                                                                    |
| `itemNotFound`          | O recurso solicitado não existe. Não é esperado que o cliente do Microsoft Graph reenvie a solicitação com falha.                                                                                                                                                                                                                         |
| `methodNotAllowed`      | O método HTTP especificado na solicitação não é permitido no recurso. Não é esperado que o cliente do Microsoft Graph reenvie a solicitação com falha.                                                                                                                                                                                      |
| `nonBlankCellOffSheet`  | Não é possível inserir novas células porque ele efetuaria push de células não vazias para fora do final da planilha. Não é esperado que o cliente do Microsoft Graph reenvie a solicitação com falha. Um usuário final pode excluir linhas ou colunas para abrir espaço para que o conteúdo seja inserido e tente novamente.                                                                 |
| `rangeExceedsLimit`     | A contagem de células no intervalo excedeu o número máximo com suporte. O cliente do Microsoft Graph pode tentar enviar uma solicitação com tamanho de intervalo menor. Para obter mais informações, [consulte Limites de recursos e otimização de desempenho para Suplementos do Office](/office/dev/add-ins/concepts/resource-limits-and-performance-optimization#excel-add-ins). |
| `requestAborted`        | A solicitação foi anulada durante o tempo de execução, o que geralmente foi causado pelo cálculo de tempo longo das funções na pasta de trabalho. Não é esperado que o cliente do Microsoft Graph reenvie a solicitação com falha.                                                                                                                                    |
| `unsupportedOperation`  | Não há suporte para a operação que está sendo tentada. Não é esperado que o cliente do Microsoft Graph reenvie a solicitação com falha.                                                                                                                                                                                                               |

> [!NOTE]
> Para o padrão regular, a solicitação com falha é definida como a solicitação que corresponde à resposta. Para o padrão de operação de execução longa, a solicitação com falha é aquela que dispara a operação com falha.

### <a name="3-parse-the-top-level-error-code"></a>3. Analisar o código de erro de nível superior

Se você não encontrar nenhum código de erro de segundo nível conhecido, siga as instruções fornecidas para erros de nível superior. Os códigos de erro de nível superior são associados ao código de status e você pode executar uma ação de acordo com os códigos de status correspondentes. Para obter detalhes sobre códigos de erro e mensagens de nível superior, consulte [Códigos de erro e mensagens](workbook-error-codes.md#error-codes-and-messages).

### <a name="4-parse-the-status-code"></a>4. Analisar o código de status

Para o padrão regular, se você não conseguiu encontrar nenhum código de erro de segundo nível conhecido ou código de erro de nível superior, deverá executar uma ação de acordo com o código de status HTTP.

### <a name="5-error-recovery-cooldown"></a>5. Resfriamento da recuperação de erro

Para algumas das respostas no padrão regular, uma duração de resfriamento de recuperação em segundos pode ser fornecida por meio de um `Retry-After` cabeçalho. Quando uma duração de resfriamento de recuperação está presente, o cliente do Microsoft Graph não deve enviar nenhuma solicitação de acompanhamento antes que a duração especificada passe. Para obter as práticas recomendadas `Retry-After` relacionadas ao cabeçalho e à limitação, consulte [Reduzir erros de limitação](workbook-best-practice.md#reduce-throttling-errors).

## <a name="diagnostic-information"></a>Informações de diagnóstico

Todo o conteúdo na resposta que não é usado nas etapas anteriores é apenas para fins de diagnóstico (incluindo cadeias de caracteres nos campos **de** mensagem). Não recomendamos que você use uma dependência desses conteúdos, pois eles podem mudar sem aviso prévio.

## <a name="special-case-handling"></a>Tratamento de caso especial

Para [solicitações de](excel-manage-sessions.md#request-types) sessão, `502/badGateway` `503/serviceUnavailable` se você encontrar um ou erro, quando um código de erro de segundo nível conhecido for encontrado, siga as instruções correspondentes; caso contrário, recrie a sessão diretamente.
<!-- {
  "type": "#page.annotation",
  "description": "Error handling in Excel Graph.",
  "keywords": "error response, error object, error codes, innerError, error handling",
  "section": "documentation",
  "tocPath": ""
} -->

## <a name="see-also"></a>Confira também

- [Usar a API REST do Excel](/graph/api/resources/excel)
