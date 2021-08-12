---
title: Usar a API do Microsoft Graph
description: O Microsoft Graph é uma API Web RESTful que permite que você acesse os recursos de serviço do Microsoft Cloud. Depois que você registrar seu aplicativo e obter tokens de autenticação para um usuário ou serviço, é possível fazer solicitações para a API do Microsoft Graph.
author: jackson-woods
localization_priority: Priority
ms.custom: graphiamtop20, scenarios:getting-started
ms.openlocfilehash: 6fc4de0eba8feb09668d0b1fd5b059dc6c9f3140a02bf4f99ae31743e1a9d5f2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54157870"
---
# <a name="use-the-microsoft-graph-api"></a>Usar a API do Microsoft Graph

O Microsoft Graph é uma API Web RESTful que permite que você acesse os recursos de serviço do Microsoft Cloud. Depois que você [registrar seu aplicativo](auth-register-app-v2.md) e [obter tokens de autenticação para um usuário](auth-v2-user.md) ou [serviço](auth-v2-service.md), é possível fazer solicitações para a API do Microsoft Graph.

> **Importante:**  a maneira como políticas de acesso condicional se aplicam ao Microsoft Graph está mudando. Os aplicativos precisam ser atualizados para lidar com cenários em que as políticas de acesso condicional são configuradas. Para obter mais informações e orientações, confira [Diretrizes de desenvolvedor para acesso condicional do Azure Active Directory](/azure/active-directory/develop/active-directory-conditional-access-developer).

## <a name="odata-namespace"></a>Espaço de nomes (namespace) OData

A API do Microsoft Graph define a maioria dos seus recursos, métodos e enumerações no namespace OData, `microsoft.graph`nos [metadados do Microsoft Graph](traverse-the-graph.md#microsoft-graph-api-metadata). Um pequeno número de conjuntos de APIs são definidos em seus subnamespaces, como a [API de registros de chamada](/graph/api/resources/callrecords-api-overview), que define recursos como [callRecord](/graph/api/resources/callrecords-callrecord) no `microsoft.graph.callRecords`. 

A menos que especificado explicitamente no tópico correspondente, considere tipos, métodos e enumerações fazem parte do espaço de nomes `microsoft.graph`.

## <a name="call-a-rest-api-method"></a>Método de chamada à API REST

Para ler de ou gravar em um recurso como um usuário ou uma mensagem de email, você constrói uma solicitação semelhante ao visto abaixo:

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

Estamos sempre buscando comentários sobre nossas APIs beta. Para enviar comentários ou solicitar recursos, confira nossa página [fórum de ideias da plataforma de desenvolvedores do Microsoft 365](https://techcommunity.microsoft.com/t5/microsoft-365-developer-platform/idb-p/Microsoft365DeveloperPlatform/label-name/Microsoft%20Graph).

Para saber mais sobre as versões da API, veja [Suporte e controle de versão](versioning-and-support.md).

## <a name="resource"></a>Recurso

Um recurso pode ser uma entidade ou tipo complexo, normalmente definido com propriedades. As entidades são diferentes de tipos complexos, incluindo sempre uma propriedade de **id**.

Sua URL incluirá um ou mais recursos com os quais você está interagindo, como `me`, **usuário**, **grupo**, **unidade** e **site**. Muitas vezes, os recursos de nível superior também incluem _relações_, que você pode usar para acessar recursos adicionais, como `me/messages` ou `me/drive`. Você também pode interagir com os recursos usando _métodos_; para enviar um email, use `me/sendMail`. Para obter mais informações, confira [Acessar dados e métodos navegando no Microsoft Graph](traverse-the-graph.md).

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

Com exceção das opções de consulta OData, alguns métodos exigem valores de parâmetro especificados como parte da URL da consulta. Por exemplo, é possível obter uma coleção de eventos ocorridos durante um período de tempo no calendário de um usuário, consultando a relação **calendarView** de um **usuário** e especificando o período dos valores `startDateTime` e `endDateTime` como parâmetros da consulta:

<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/me/calendarView?startDateTime=2019-09-01T09:00:00.0000000&endDateTime=2019-09-01T17:00:00.0000000
```

## <a name="tools-for-interacting-with-microsoft-graph"></a>Ferramentas para interagir com o Microsoft Graph

### <a name="graph-explorer"></a>Explorador do Graph

O Explorador do Graph é uma ferramenta baseada na Web que você pode usar para criar e testar solicitações usando as APIs do Microsoft Graph. Você pode acessar o Explorador do Graph em: [https://developer.microsoft.com/graph/graph-explorer](https://developer.microsoft.com/graph/graph-explorer).

Você pode acessar os dados de demonstração sem fazer logon, ou pode fazer logon em um locatário de sua preferência. Use as etapas a seguir para criar a solicitação:

1. Selecione o método HTTP.
2. Selecione a versão da API que você deseja usar.
3. Digite a consulta na caixa de texto da solicitação.
4. Selecione **Executar consulta**. 

O exemplo a seguir mostra uma solicitação que retorna informações sobre usuários no locatário da demonstração:

![Captura de tela do Explorador do Graph com uma solicitação de usuário GET realçada](./images/graph-explorer.png)

Os exemplos de consultas são fornecidos no Explorador do Graph para permitir que você execute solicitações comuns mais rapidamente. Para ver os exemplos disponíveis, selecione **mostrar mais exemplos**. Selecione **Ativado** para o conjunto de exemplos que deseja ver e, depois de fechar a janela de seleção, você deverá ver uma lista de solicitações predefinidas.

Um código de status e uma mensagem são exibidos depois que uma solicitação é enviada, e a resposta é exibida na guia **Visualização de resposta**.

### <a name="postman"></a>Postman

O Postman é uma ferramenta que você pode usar para criar e testar solicitações usando as APIs do Microsoft Graph. Você pode baixar o Postman em: [https://www.getpostman.com/](https://www.getpostman.com/). Para interagir com o Microsoft Graph no Postman, use a coleção do Microsoft Graph.

Para obter mais informações, confira [Usar o Postman com a API do Microsoft Graph](./use-postman.md).

## <a name="next-steps"></a>Próximas etapas

Você está pronto para começar a usar o Microsoft Graph. Experimente o [Início rápido](https://developer.microsoft.com/graph/quick-start) ou comece usando um de nossos [SDKs e exemplos de código](https://developer.microsoft.com/graph/code-samples-and-sdks).
