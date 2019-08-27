---
title: Usar a API do Microsoft Graph
description: O Microsoft Graph é uma API Web RESTful que permite que você acesse os recursos de serviço do Microsoft Cloud. Depois que você registrar seu aplicativo e obter tokens de autenticação para um usuário ou serviço, é possível fazer solicitações para a API do Microsoft Graph.
author: jackson-woods
localization_priority: Priority
ms.openlocfilehash: 9f95868069c2ffd404076e5b3baf572e21b61eeb
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/27/2019
ms.locfileid: "36633241"
---
# <a name="use-the-microsoft-graph-api"></a>Usar a API do Microsoft Graph

O Microsoft Graph é uma API Web RESTful que permite que você acesse os recursos de serviço do Microsoft Cloud. Depois que você [registrar seu aplicativo](auth-register-app-v2.md) e [obter tokens de autenticação para um usuário](auth-v2-user.md) ou [serviço](auth-v2-service.md), é possível fazer solicitações para a API do Microsoft Graph.

> **Importante:**  a maneira como políticas de acesso condicional se aplicam ao Microsoft Graph está mudando. Os aplicativos precisam ser atualizados para lidar com cenários em que as políticas de acesso condicional são configuradas. Para obter mais informações e orientações, confira [Diretrizes de desenvolvedor para acesso condicional do Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/active-directory-conditional-access-developer).

Para ler de ou gravar em um recurso como um usuário ou uma mensagem de email, você constrói uma solicitação semelhante ao seguinte.

<!-- {
  "blockType": "ignored"
}-->
```http
{HTTP method} https://graph.microsoft.com/{version}/{resource}?{query-parameters}
```

Os componentes de uma solicitação incluem:

* [{Método HTTP}](#http-methods) – O método HTTP usado na solicitação para o Microsoft Graph.
* [{versão}](#version) – A versão da API do Microsoft Graph que seu aplicativo está usando.
* [{recurso}](#resource) – O recurso no Microsoft Graph ao qual você está fazendo referência. 
* [{Parâmetros-da-consultas}](#query-parameters) –Opções de consulta OData opcionais ou parâmetros do método REST que personalizam a resposta.

Depois de fazer uma solicitação, uma resposta é retornada, que inclui: 

* Código de status – um código de status HTTP que indica o sucesso ou o fracasso. Para obter detalhes sobre os códigos de erro HTTP, confira [Erros](errors.md).
* Mensagem de resposta – os dados que você solicitou ou o resultado da operação. A mensagem de resposta pode estar vazia em algumas operações.
* `nextLink` – Se a solicitação retornar muitos dados, será necessário percorrê-los usando a URL retornada no `@odata.nextLink`. Para obter detalhes, confira [Paginação](paging.md).

## <a name="http-methods"></a>Métodos HTTP

O Microsoft Graph usa o método HTTP em sua solicitação para determinar sua solicitação está fazendo. A API é compatível com os seguintes métodos.


|**Method** |**Descrição**                             |
| :----- | :------------------------------------------- |
| GET    | Ler dados de um recurso.                   |
| POST   | Criar um novo recurso, ou executar uma ação. |
| PATCH  | Atualizar um recurso com novos valores.           |
| PUT    | Substituir um recurso por um novo.           |
| DELETE | Remover um recurso.                           |

* Nos métodos CRUD, `GET` e `DELETE`, nenhum corpo de solicitação é obrigatório.
* Os métodos `POST`, `PATCH` e `PUT` precisam de um corpo de solicitação, normalmente especificado em formato JSON que contém informações adicionais, como os valores das propriedades do recurso.

## <a name="version"></a>Versão

O Microsoft Graph atualmente é compatível com duas versões: `v1.0` e `beta`.

* O `v1.0` inclui APIs normalmente disponíveis. Use a versão 1.0 para todos os aplicativos de produção.
* O `beta` inclui APIs que estão atualmente em modo de visualização. Como podemos apresentar alterações significativas a nossas APIs beta, recomendamos que você use a versão beta apenas para testar aplicativos em desenvolvimento. Não use APIs beta em seus aplicativos de produção.

Estamos sempre buscando comentários sobre nossas APIs beta. Para fornecer comentários ou solicitar recursos, veja nossa página [UserVoice](https://officespdev.uservoice.com/).

Para saber mais sobre as versões da API, veja [Suporte e controle de versão](versioning-and-support.md).

## <a name="resource"></a>Recurso

Um recurso pode ser uma entidade ou tipo complexo, normalmente definido com propriedades. As entidades são diferentes de tipos complexos, incluindo sempre uma propriedade de **id**.

Sua URL incluirá um ou mais recursos com que você está interagindo na solicitação, como `me`, **usuário**, **grupo**, **unidade** e **site**. Frequentemente, cada um dos recursos de nível superior também inclui _relações_, que podem ser usadas para acessar recursos adicionais, como `me/messages` ou `me/drive`. Você também pode interagir com os recursos usando _métodos_; por exemplo, para enviar um email, use `me/sendMail`. Para mais informações, confira [Acessar dados e métodos ao navegar no Microsoft Graph](traverse-the-graph.md).

Cada recurso pode exigir diferentes permissões de acesso. Muitas vezes será necessário um nível mais alto de permissões para criar ou atualizar um recurso do que para lê-lo. Para obter detalhes sobre as permissões necessárias, veja o tópico de referência do método. 

Para obter detalhes sobre permissões, veja [Referência de permissões](permissions-reference.md).

## <a name="query-parameters"></a>Parâmetros de consulta

Os parâmetros de consulta podem ser opções de consulta do sistema OData ou outras cadeias de caracteres que um método aceita para personalizar a resposta.

Use parâmetros de consulta do sistema OData para incluir mais ou menos propriedades do que a resposta padrão, filtrar a resposta para itens que correspondem a uma consulta personalizada ou oferecem parâmetros adicionais para um método.

Por exemplo, adicionar o seguinte parâmetro de `filter` restringe as mensagens retornadas para apenas aquelas com a propriedade de `emailAddress` do `jon@contoso.com`. 

<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages?filter=emailAddress eq 'jon@contoso.com'
```

Para obter mais informações sobre as opções de consulta OData, confira [Usar parâmetros de consulta para personalizar respostas](query-parameters.md).

Com exceção das opções de consulta OData, alguns métodos exigem valores de parâmetro especificados como parte da URL da consulta. Por exemplo, é possível obter uma coleção de eventos ocorridos durante um período de tempo no calendário de um usuário, consultando a relação **calendarView** de um **usuário**e especificando o período dos valores `startDateTime` e `endDateTime` como parâmetros da consulta:

<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/me/calendarView?startDateTime=2019-09-01T09:00:00.0000000&endDateTime=2019-09-01T17:00:00.0000000
```

## <a name="next-steps"></a>Próximas etapas

Você está pronto para começar a trabalhar com o Microsoft Graph. Para saber mais, vá para o [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer) para experimentar algumas solicitações, tente o [Início Rápido](https://developer.microsoft.com/graph/quick-start) ou comece a usar um dos nossos [SDKs e exemplos de código](https://developer.microsoft.com/graph/code-samples-and-sdks).
