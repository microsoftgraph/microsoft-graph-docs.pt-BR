---
title: Usar a API do Microsoft Graph
description: O Microsoft Graph é uma API Web RESTful que permite que você acesse os recursos de serviço do Microsoft Cloud. Depois que você registrar seu aplicativo e obter tokens de autenticação para um usuário ou serviço, é possível fazer solicitações para a API do Microsoft Graph.
ms.openlocfilehash: 1a9d9bcefdfb302a9de602aa15aa642a0c57a793
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27091682"
---
# <a name="use-the-microsoft-graph-api"></a>Usar a API do Microsoft Graph

O Microsoft Graph é uma API Web RESTful que permite que você acesse os recursos de serviço do Microsoft Cloud. Depois que você [registrar seu aplicativo](auth-register-app-v2.md) e [obter tokens de autenticação para um usuário](auth-v2-user.md) ou [serviço](auth-v2-service.md), é possível fazer solicitações para a API do Microsoft Graph.

> **Importante:**  A maneira como políticas de acesso condicional se aplicam ao Microsoft Graph está mudando. Os aplicativos precisam ser atualizados para lidar com cenários em que as políticas de acesso condicional são configuradas. Para obter mais informações e orientações, confira [Diretrizes de desenvolvedor para acesso condicional do Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/active-directory-conditional-access-developer).

Para ler de ou gravar em um recurso como um usuário ou uma mensagem de email, você constrói uma solicitação semelhante ao seguinte.

```http
https://graph.microsoft.com/{version}/{resource}?query-parameters
```

Os componentes de uma solicitação incluem:

* [Método HTTP](#http-methods) -o método HTTP usado na solicitação para o Microsoft Graph.
* [`{version}`](#version) – a versão da API do Microsoft Graph que seu aplicativo está usando.
* [`{resource}`](#resource) – o recurso no Microsoft Graph ao qual você está fazendo referência.
* [query-parameters](#query-parameters-optional) – um conjunto opcional de parâmetros para modificar a solicitação ou a resposta.

Depois de fazer uma solicitação, uma resposta é retornada, que inclui: 

* Código de status – um código de status HTTP que indica o sucesso ou o fracasso. Para obter detalhes sobre os códigos de erro HTTP, veja [Erros](errors.md).
* Mensagem de resposta – os dados que você solicitou ou o resultado da operação. A mensagem de resposta pode estar vazia em algumas operações.
* Link **Avançar** – se a solicitação retornar muitos dados, você precisa percorrê-los escolhendo **Avançar**. Para obter detalhes, veja [Paginação](paging.md).

## <a name="http-methods"></a>Métodos HTTP

O Microsoft Graph usa o método HTTP em sua solicitação para determinar sua solicitação está fazendo. A API é compatível com os seguintes métodos.


|**Method** |**Descrição**                             |
| :----- | :------------------------------------------- |
| GET    | Ler dados de um recurso.                   |
| POST   | Criar um novo recurso, ou executar uma ação. |
| PATCH  | Atualizar um recurso com novos valores.           |
| PUT    | Substituir um recurso por um novo.           |
| DELETE | Remover um recurso.                           |

* Nos métodos **GET** e **DELETE**, nenhum corpo de solicitação é obrigatório.
* Os métodos **POST**, **PATCH** e **PUT** precisam de um corpo de solicitação, normalmente especificado em formato JSON que contém informações adicionais, como os valores das propriedades do recurso.

## <a name="version"></a>Versão

O Microsoft Graph atualmente é compatível com duas versões: `v1.0` e `beta`.

* O `v1.0` inclui APIs normalmente disponíveis. Use a versão 1.0 para todos os aplicativos de produção.
* O `beta` inclui APIs que estão atualmente em modo de visualização. Como podemos apresentar alterações significativas a nossas APIs beta, recomendamos que você use a versão beta apenas para testar aplicativos em desenvolvimento. Não use APIs beta em seus aplicativos de produção.

Estamos sempre buscando comentários sobre nossas APIs beta. Para fornecer comentários ou solicitar recursos, veja nossa página [UserVoice](https://officespdev.uservoice.com/).

Para saber mais sobre as versões da API, veja [Suporte e controle de versão](versioning-and-support.md).

## <a name="resource"></a>Recurso

Sua URL incluirá um ou mais recursos com que você está interagindo na solicitação, como `me`, `users`, `groups`, `drives` e `sites`. Cada um dos recursos de nível superior também inclui **relações**, que podem ser usados para acessar recursos adicionais, como `me/messages` ou `me/drive`. Você também pode interagir com os recursos usando **métodos**, por exemplo, para enviar um email, use `me/sendMail`.

Para saber mais sobre como navegar por métodos e relações do recurso, confira [Desviar o gráfico](traverse-the-graph.md). 

Cada recurso pode exigir diferentes permissões de acesso. Muitas vezes será necessário um nível mais alto de permissões para criar ou atualizar um recurso do que para lê-lo. Para obter detalhes sobre as permissões necessárias, veja o tópico de referência do método. 

Para obter detalhes sobre permissões, veja [Referência de permissões](permissions-reference.md).

## <a name="query-parameters-optional"></a>Parâmetros de consulta (opcional)

Você pode usar parâmetros de consulta opcionais para personalizar a resposta em seu aplicativo Microsoft Graph. Use parâmetros de consulta para incluir mais ou menos propriedades do que a resposta padrão, filtrar a resposta para itens que correspondem a uma consulta personalizada ou oferecem parâmetros adicionais para um método.

Por exemplo, adicionar o seguinte parâmetro de filtro restringe as mensagens retornadas para apenas aquelas com a propriedade `emailAddress` de `jon@contoso.com`.

```http
https://graph.microsoft.com/v1.0/me/messages?filter=emailAddress eq 'jon@contoso.com'
```

Para saber mais sobre os parâmetros de consulta, veja [Personalizar respostas](query-parameters.md).

## <a name="next-steps"></a>Próximas etapas

Você está pronto para começar a trabalhar com o Microsoft Graph. Para saber mais, vá para o [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer) para experimentar algumas solicitações, tente o [Início Rápido](https://developer.microsoft.com/graph/quick-start) ou comece a usar um dos nossos [SDKs e exemplos de código](https://developer.microsoft.com/graph/code-samples-and-sdks).
