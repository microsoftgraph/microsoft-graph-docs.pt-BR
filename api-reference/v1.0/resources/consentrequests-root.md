---
title: Solicitações de consentimento do Azure Active Directory
description: Use as solicitações de consentimento do Azure AD para gerenciar o fluxo de trabalho de solicitação para usuários que tentam acessar aplicativos que exigem consentimento do administrador.
localization_priority: Normal
author: psignoret
ms.prod: governance
doc_type: conceptualPageType
ms.openlocfilehash: d9d19a3756ac39fef061584e97ad55e4a4c12aff
ms.sourcegitcommit: ad1e4d758d4fe6025987c1c3528ce644edb27062
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/13/2021
ms.locfileid: "51698045"
---
# <a name="azure-active-directory-consent-requests"></a>Solicitações de consentimento do Azure Active Directory

Namespace: microsoft.graph

As solicitações de consentimento do Azure Active Directory (Azure AD) ajudam você a gerenciar o fluxo de trabalho de solicitação para usuários que tentam acessar aplicativos que exigem aprovação do administrador.

Para permitir que os usuários solicitem acesso ou consentimento de administrador para aplicativos que não estão autorizados a conceder consentimento a si mesmos, primeiro habilita o fluxo de trabalho de solicitação de consentimento. 

>[!NOTE]
>As APIs atuais estão limitadas a configurar o fluxo de trabalho, ler a lista de solicitações e negar uma solicitação. No momento, não há métodos disponíveis para aprovar programaticamente uma solicitação. No entanto, o conteúdo da solicitação pode ser usado para recriar uma URL que pode ser usada para conceder o consentimento do administrador e aprovar uma solicitação.

Os tipos de recursos de solicitação de consentimento incluem:

* [adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md): especifica a política pela qual as solicitações de consentimento do aplicativo podem ser criadas e gerenciadas para todo o locatário. Há um único **adminConsentRequestPolicy** por locatário.
* [appConsentRequest](../resources/appconsentrequest.md): uma solicitação que representa uma coleção de **objetos userConsentRequest** para um aplicativo específico.
* [userConsentRequest](../resources/userconsentrequest.md): uma solicitação criada por um usuário para usar um aplicativo que exige o consentimento do administrador para acessar.
* [appConsentRequestScope](../resources/appconsentrequestscope.md): um recurso que contém detalhes dos escopos de permissão dinâmicos que estão sendo solicitados para um aplicativo.  

## <a name="methods"></a>Métodos

A tabela a seguir lista os métodos que você pode usar para interagir com recursos de solicitação de consentimento.

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter adminConsentRequestPolicy](../api/adminconsentrequestpolicy-get.md) | [coleção adminConsentRequestPolicy](adminconsentrequestpolicy.md) | Leia as propriedades do [adminConsentRequestPolicy](adminconsentrequestpolicy.md). |
|[Atualizar adminConsentRequestPolicy](../api/adminconsentrequestpolicy-update.md) | [coleção adminConsentRequestPolicy](adminconsentrequestpolicy.md) | Definir configurações para [adminConsentRequestPolicy](adminconsentrequestpolicy.md). |
|[Listar appConsentRequests ](../api/appconsentrequest-list.md) | [Coleção appConsentRequest](appconsentrequest.md) | Recupere uma coleção de [objetos appConsentRequest.](appconsentrequest.md) |
|[Obter appConsentRequests ](../api/appconsentrequest-get.md) | [Coleção appConsentRequest](appconsentrequest.md) | Leia um [objeto appConsentRequest.](appconsentrequest.md) |
|[appConsentRequest: filterByCurrentUser](../api/appconsentrequest-filterByCurrentUser.md) | [Coleção appConsentRequests](../resources/appconsentrequest.md) | Leia as propriedades dos [objetos appConsentRequest](../resources/appconsentrequest.md) para os quais o usuário atual é o revistor e o status da solicitação de consentimento do usuário é `InProgress` . |
|[Obter userConsentRequest ](../api/userconsentrequest-get.md) | [Coleção userConsentRequest](userconsentrequest.md) | Leia um [objeto userConsentRequest](userconsentrequest.md) para um [appConsentRequest](appconsentrequest.md). |
|[Listar userConsentRequests ](../api/userconsentrequest-list.md) | [Coleção userConsentRequest](userconsentrequest.md) | Recupere uma coleção de [objetos userConsentRequest](userconsentrequest.md) para [um appConsentRequest](appconsentrequest.md). |
|[userConsentRequest: filterByCurrentUser](../api/userconsentrequest-filterByCurrentUser.md) | [Coleção appConsentRequests](../resources/userconsentrequest.md) | Leia as propriedades [dos objetos userConsentRequest](../resources/userconsentrequest.md) para os quais o usuário atual é o revistor. |

## <a name="role-and-delegated-permission-authorization-checks"></a>Role and delegated permission authorization checks

As seguintes funções de diretório são necessárias para que um usuário de chamada gerencie o fluxo de trabalho de solicitações ou leia a lista de solicitações.

| Operação | Permissões delegadas | Função de diretório necessária do usuário chamador |
|:------------------|:------------|:--------------------------------------------|
| Ler | ConsentRequest.Read.All, ConsentRequest.ReadWrite.All | Administrador Global, Leitor Global, Administrador de Aplicativos na Nuvem e Administrador de Aplicativos |
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
