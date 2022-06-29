---
title: Solicitações de consentimento do Azure Active Directory
description: Use Azure AD de consentimento para gerenciar o fluxo de trabalho de solicitação para usuários que tentam acessar aplicativos que exigem consentimento do administrador.
ms.localizationpriority: medium
author: psignoret
ms.prod: governance
doc_type: conceptualPageType
ms.openlocfilehash: abac5b526601ad4aec522be707e24c210f1f8f3a
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66442861"
---
# <a name="azure-active-directory-consent-requests"></a>Solicitações de consentimento do Azure Active Directory

Namespace: microsoft.graph

As solicitações de consentimento do Azure Active Directory (Azure AD) ajudam você a gerenciar o fluxo de trabalho de solicitação para usuários que tentam acessar aplicativos que exigem aprovação do administrador.

Para permitir que os usuários solicitem acesso ou consentimento do administrador para aplicativos que não estão autorizados a conceder consentimento a si mesmos, primeiro habilite o fluxo de trabalho de solicitação de consentimento. 

>[!NOTE]
>As APIs atuais estão limitadas à configuração do fluxo de trabalho e à leitura da lista de solicitações. No momento, não há nenhum método disponível para aprovar ou negar uma solicitação programaticamente. No entanto, o conteúdo da solicitação pode ser usado para recriar uma URL que pode ser usada para conceder consentimento do administrador e aprovar uma solicitação.

[!INCLUDE [GDPR-related-guidance](../../includes/gdpr-msgraph-export-note.md)]

Os tipos de recursos de solicitação de consentimento incluem:

* [adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md): especifica a política pela qual as solicitações de consentimento do aplicativo podem ser criadas e gerenciadas para todo o locatário. Há um único **adminConsentRequestPolicy** por locatário.
* [appConsentRequest](../resources/appconsentrequest.md): uma solicitação que representa uma coleção de **objetos userConsentRequest** para um aplicativo específico.
* [userConsentRequest](../resources/userconsentrequest.md): uma solicitação criada por um usuário para usar um aplicativo que requer consentimento do administrador para acessar.
* [appConsentRequestScope](../resources/appconsentrequestscope.md): um recurso que contém detalhes dos escopos de permissão dinâmica que estão sendo solicitados para um aplicativo.  

## <a name="methods"></a>Métodos

A tabela a seguir lista os métodos que você pode usar para interagir com recursos de solicitação de consentimento.

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter adminConsentRequestPolicy](../api/adminconsentrequestpolicy-get.md) | [coleção adminConsentRequestPolicy](adminconsentrequestpolicy.md) | Leia as propriedades do [adminConsentRequestPolicy](adminconsentrequestpolicy.md). |
|[Atualizar adminConsentRequestPolicy](../api/adminconsentrequestpolicy-update.md) | [coleção adminConsentRequestPolicy](adminconsentrequestpolicy.md) | Defina configurações para [adminConsentRequestPolicy](adminconsentrequestpolicy.md). |
|[Listar appConsentRequests ](../api/appconsentapprovalroute-list-appconsentrequests.md) | [coleção appConsentRequest](appconsentrequest.md) | Recupere uma coleção de [objetos appConsentRequest](appconsentrequest.md) . |
|[Obter appConsentRequests ](../api/appconsentrequest-get.md) | [coleção appConsentRequest](appconsentrequest.md) | Leia um [objeto appConsentRequest](appconsentrequest.md) . |
|[appConsentRequest: filterByCurrentUser](../api/appconsentrequest-filterByCurrentUser.md) | [Coleção appConsentRequests](../resources/appconsentrequest.md) | Leia as propriedades dos [objetos appConsentRequest](../resources/appconsentrequest.md) para os quais o usuário atual é o revisores e o status da solicitação de consentimento do usuário é `InProgress`. |
|[Obter userConsentRequest ](../api/userconsentrequest-get.md) | [coleção userConsentRequest](userconsentrequest.md) | Leia um [objeto userConsentRequest](userconsentrequest.md) para [um appConsentRequest](appconsentrequest.md). |
|[Listar userConsentRequests ](../api/appconsentrequest-list-userconsentrequests.md) | [coleção userConsentRequest](userconsentrequest.md) | Recupere uma coleção de [objetos userConsentRequest](userconsentrequest.md) para [um appConsentRequest](appconsentrequest.md). |
|[userConsentRequest: filterByCurrentUser](../api/userconsentrequest-filterByCurrentUser.md) | [Coleção appConsentRequests](../resources/userconsentrequest.md) | Leia as propriedades dos [objetos userConsentRequest](../resources/userconsentrequest.md) para os quais o usuário atual é o revistor. |

## <a name="role-and-delegated-permission-authorization-checks"></a>Verificações de autorização de função e permissão delegada

As funções de diretório a seguir são necessárias para que um usuário chamador gerencie o fluxo de trabalho de solicitações ou leia a lista de solicitações.

| Operation | Permissões delegadas | Função de diretório necessária do usuário chamador |
|:------------------|:------------|:--------------------------------------------|
| Leitura | ConsentRequest.Read.All, ConsentRequest.ReadWrite.All | Administrador Global, Leitor Global, Administrador de Aplicativos de Nuvem e Administrador de Aplicativos |

## <a name="see-also"></a>Confira também

- [Configurar o fluxo de trabalho de consentimento do administrador (versão prévia)](/azure/active-directory/manage-apps/configure-admin-consent-workflow?preserve-view=true)


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
