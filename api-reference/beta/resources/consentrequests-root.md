---
title: Solicitações de consentimento do Azure Active Directory
description: Use as solicitações de consentimento do Azure AD para gerenciar o fluxo de trabalho de solicitação para usuários que tentam acessar aplicativos que exigem consentimento do administrador.
localization_priority: Normal
author: psignoret
ms.prod: governance
doc_type: conceptualPageType
ms.openlocfilehash: e572b2b80ebe2e4a62395431f8b24ab89cc63614
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50965024"
---
# <a name="azure-active-directory-consent-requests"></a>Solicitações de consentimento do Azure Active Directory

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

As solicitações de consentimento do Azure Active Directory (Azure AD) ajudam você a gerenciar o fluxo de trabalho de solicitação para usuários que tentam acessar aplicativos que exigem aprovação do administrador.

Para permitir que os usuários solicitem acesso ou consentimento de administrador para aplicativos que não estão autorizados a conceder consentimento a si mesmos, primeiro habilita o fluxo de trabalho de solicitação de consentimento. 

>[!NOTE]
>As APIs atuais estão limitadas a configurar o fluxo de trabalho, ler a lista de solicitações e negar uma solicitação. No momento, não há métodos disponíveis para aprovar uma solicitação programaticamente. No entanto, o conteúdo da solicitação pode ser usado para recriar uma URL que pode ser usada para conceder o consentimento do administrador e aprovar uma solicitação.

Os tipos de recursos de solicitação de consentimento incluem:

* [adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md): especifica a política pela qual as solicitações de consentimento do aplicativo podem ser criadas e gerenciadas para todo o locatário. Há um único **adminConsentRequestPolicy** por locatário.
* [appConsentRequest](../resources/appconsentrequest.md): uma solicitação que representa uma agregação de **userConsentRequests** para um aplicativo específico.
* [userConsentRequest](../resources/userconsentrequest.md): uma solicitação criada por um usuário para usar um aplicativo que exige o consentimento do administrador para acessar.
* [appConsentRequestScope](../resources/appconsentrequestscope.md): um recurso que contém detalhes dos escopos de permissão dinâmicos que estão sendo solicitados para um determinado aplicativo.  


## <a name="methods"></a>Métodos

A tabela a seguir lista os métodos que você pode usar para interagir com recursos de solicitação de consentimento.

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter adminConsentRequestPolicy](../api/adminconsentrequestpolicy-get.md) | [coleção adminConsentRequestPolicy](adminconsentrequestpolicy.md) | Ler as propriedades do [adminConsentRequestPolicy](adminconsentrequestpolicy.md) |
|[Atualizar adminConsentRequestPolicy](../api/adminconsentrequestpolicy-update.md) | [coleção adminConsentRequestPolicy](adminconsentrequestpolicy.md) | Definir configurações para [o adminConsentRequestPolicy](adminconsentrequestpolicy.md) |
|[Listar appConsentRequests ](../api/appconsentrequest-list.md) | [Coleção appConsentRequest](appconsentrequest.md) | Recuperar uma lista de [todos os appConsentRequests](appconsentrequest.md) |
|[Obter appConsentRequests ](../api/appconsentrequest-get.md) | [Coleção appConsentRequest](appconsentrequest.md) | Ler um determinado [appConsentRequest](appconsentrequest.md) |
|[Listar appConsentRequests: filterByCurrentUser](../api/appconsentrequest-filterByCurrentUser.md) | [Coleção appConsentRequests](../resources/appconsentrequest.md) | Leia as propriedades do [appConsentRequests](../resources/appconsentrequest.md) para os quais o usuário atual é o revistor e o status da solicitação de consentimento do usuário é `InProgress` . |
|[Obter userConsentRequests ](../api/userconsentrequest-get.md) | [Coleção userConsentRequest](userconsentrequest.md) | Recuperar um [dado userConsentRequests](userconsentrequest.md) para um [determinado appConsentRequest](appconsentrequest.md) |
|[Listar userConsentRequests ](../api/userconsentrequest-list.md) | [Coleção userConsentRequest](userconsentrequest.md) | Recuperar uma lista de [todos os userConsentRequests](userconsentrequest.md) para um [determinado appConsentRequest](appconsentrequest.md) |
|[Listar userConsentRequests: filterByCurrentUser](../api/userconsentrequest-filterByCurrentUser.md) | [Coleção appConsentRequests](../resources/userconsentrequest.md) | Leia as propriedades do [userConsentRequests](../resources/userconsentrequest.md) para os quais o usuário atual é o revistor e o status da solicitação de consentimento do usuário é `InProgress` . |

## <a name="role-and-delegated-permission-authorization-checks"></a>Role and delegated permission authorization checks

As seguintes funções de diretório são necessárias para que um usuário de chamada gerencie o fluxo de trabalho de solicitações ou leia a lista de solicitações.

| Operation | Permissões delegadas | Função de diretório necessária do usuário chamador |
|:------------------|:------------|:--------------------------------------------|
| Leitura | ConsentRequest.Read.All, ConsentRequest.ReadWrite.All | Administrador Global, Leitor Global, Administrador de Aplicativos na Nuvem e Administrador de Aplicativos |
| Atualizar | ConsentRequest.ReadWrite.All |Administrador Global |

## <a name="see-also"></a>Confira também

- [Configurar o fluxo de trabalho de consentimento do administrador (visualização)](/azure/active-directory/manage-apps/configure-admin-consent-workflow?preserve-view=true)


<!--
{
  "type": "#page.annotation",
  "description": "Service root",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
