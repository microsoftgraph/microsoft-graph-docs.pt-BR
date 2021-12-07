---
title: Trabalhando com a API de gerenciamento de direitos do Azure AD
description: Governe o acesso a recursos, incluindo grupos, aplicativos e sites por meio do gerenciamento de direitos do Azure AD
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: conceptualPageType
ms.openlocfilehash: 38d30da6d55ebdff4abb55d584b4c0cb7d59a9fa
ms.sourcegitcommit: f65eee432cc903324b5f9b31710fdc6100590f36
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/07/2021
ms.locfileid: "61322006"
---
# <a name="working-with-the-azure-ad-entitlement-management-api"></a>Trabalhando com a API de gerenciamento de direitos do Azure AD

Namespace: microsoft.graph

Azure Active Directory (Azure AD) gerenciamento de direitos pode ajudá-lo a gerenciar o acesso a grupos, aplicativos e sites SharePoint Online para usuários internos, bem como usuários fora da sua organização.

Ao criar pacotes de acesso com as funções que os usuários precisam ter nesses recursos e definir políticas para quem pode solicitar um pacote de acesso e por quanto tempo eles podem ter uma atribuição para um pacote de acesso, você pode reger o ciclo de vida do acesso para usuários internos e externos.

Os tipos de recursos de gerenciamento de direitos incluem:

- [accessPackage](accesspackage.md): define as coleções de funções de recurso e as políticas de como um ou mais usuários podem obter acesso a esses recursos.
- accessPackageAssignmentPolicy: Especifica a política pela qual os titulares podem solicitar ou ter um pacote de acesso atribuído por meio de uma atribuição de pacote de acesso.
- [accessPackageAssignmentRequest](accesspackageassignmentrequest.md): Criado por um usuário que deseja obter uma atribuição de pacote de acesso.
- [accessPackageAssignment](accesspackageassignment.md): Uma atribuição de um pacote de acesso a um assunto específico, por um período de tempo.
- [accessPackageCatalog](accesspackagecatalog.md): um contêiner para pacotes de acesso.
- [connectedOrganization](connectedorganization.md): uma organização conectada para usuários externos que podem solicitar acesso.
- [entitlementManagementSettings](entitlementmanagementsettings.md): configurações de todo o locatário para o gerenciamento de direitos do Azure AD.
- [aprovação](approval.md): representa as decisões associadas a uma solicitação de pacote de acesso.

Observe que o recurso de gerenciamento de direitos, incluindo a API, está incluído Azure AD Premium P2. O locatário em que o gerenciamento de direitos está sendo usado deve ter uma assinatura de compra ou avaliação válida Azure AD Premium P2 ou EMS E5.

A tabela a seguir lista os métodos que você pode usar para interagir com recursos relacionados ao gerenciamento de direitos.

## <a name="methods"></a>Methods

| Método   | Tipo de retorno |Descrição|
|:---------------|:--------|:----------|
| [Get](../api/entitlementmanagementsettings-get.md) | [entitlementManagementSettings](entitlementmanagementsettings.md) | Leia as propriedades de **um objeto entitlementManagementSettings.** |
| [Atualizar](../api/entitlementmanagementsettings-update.md) | [entitlementManagementSettings](entitlementmanagementsettings.md) | Atualize as propriedades de **um objeto entitlementManagementSettings.** |
| [Listar accessPackages](../api/entitlementmanagement-list-accesspackages.md) | [Coleção accessPackage](accesspackage.md) | Recupere uma lista de **objetos accessPackage.** |
| [Criar accessPackage](../api/entitlementmanagement-post-accesspackages.md) | [accessPackage](accesspackage.md) | Crie um novo **objeto accessPackage.** |
| [Obter accessPackage](../api/accesspackage-get.md) | [accessPackage](accesspackage.md) | Ler propriedades e relações de um **objeto accessPackage.** |
| [Atualizar accessPackage](../api/accesspackage-update.md)|Nenhum | Atualize as propriedades de um **objeto accesspackage.** |
| [Excluir accessPackage](../api/accesspackage-delete.md) | | Excluir **accessPackage**. |
| [FilterByCurrentUser](../api/accesspackage-filterbycurrentuser.md) | [Coleção accessPackage](accesspackage.md) | Recupere uma lista de **objetos accessPackage** filtrados no usuário de entrada. |
| [Listar accessPackageAssignmentRequests](../api/entitlementmanagement-list-assignmentrequests.md) | [coleção accessPackageAssignmentRequest](accesspackageassignmentrequest.md) | Recupere uma lista de **objetos accessPackageAssignmentRequest.** |
| [Criar accessPackageAssignmentRequest](../api/entitlementmanagement-post-assignmentrequests.md) | [accessPackageAssignmentRequest](accesspackageassignmentrequest.md) | Cria um novo **objeto accessPackageAssignmentRequest.** |
| [Obter accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-get.md) | [accessPackageAssignmentRequest](accesspackageassignmentrequest.md) | Leia propriedades e relações de um **objeto accessPackageAssignmentRequest.** |
| [Excluir accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-delete.md) |Nenhum | Excluir um **accessPackageAssignmentRequest**. |
|[FilterByCurrentUser](../api/accesspackageassignmentrequest-filterbycurrentuser.md)|[coleção accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md)|Recupere a lista de **objetos accessPackageAssignmentRequest** filtrados no usuário de entrada.|
|[cancel](../api/accesspackageassignmentrequest-cancel.md)|[coleção accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md)|Cancele **um objeto accessPackageAssignmentRequest** que está em estado cancelável: `accepted` , , , `pendingApproval` `pendingNotBefore` `pendingApprovalEscalated` .|
| [Listar accessPackageAssignments](../api/entitlementmanagement-list-assignments.md) | [Coleção accessPackageAssignment](accesspackageassignment.md) | Recupere uma lista de **objetos accessPackageAssignment.** |
|[FilterByCurrentUser](../api/accesspackageassignment-filterbycurrentuser.md)|[Coleção accessPackageAssignment](../resources/accesspackageassignment.md)|Recupere a lista de **objetos accessPackageAssignment** filtrados no usuário de entrada.|
| [Listar accessPackageCatalogs](../api/entitlementmanagement-list-catalogs.md) | [Coleção accessPackageCatalog](accesspackagecatalog.md) | Recupere uma lista de **objetos accessPackageCatalogs.** |
| [Criar accessPackageCatalog](../api/entitlementmanagement-post-catalogs.md) | [accessPackageCatalog](accesspackagecatalog.md) | Crie um novo **objeto accessPackageCatalog.** |
| [Obter accessPackageCatalog](../api/accesspackagecatalog-get.md) | [accessPackageCatalog](accesspackagecatalog.md) | Ler propriedades e relações de um **objeto accessPackageCatalog.** |
| [Atualizar accessPackageCatalog](../api/accesspackagecatalog-update.md)|Nenhum | Atualize as propriedades de um **objeto accessPackageCatalog.** |
| [Excluir accessPackageCatalog](../api/accesspackagecatalog-delete.md) | | Excluir um **accessPackageCatalog**. |
| [Listar connectedOrganizations](../api/entitlementmanagement-list-connectedorganizations.md) | [Coleção connectedOrganization](connectedorganization.md) | Recupere uma lista de **objetos connectedOrganization.** |
| [Criar connectedOrganization](../api/entitlementmanagement-post-connectedorganizations.md) | [connectedOrganization](connectedorganization.md) | Crie um novo **objeto connectedOrganization.** |
| [Obter connectedOrganization](../api/connectedorganization-get.md) | [connectedOrganization](connectedorganization.md) | Leia propriedades e relações de um **objeto connectedOrganization.** |
| [Atualizar connectedOrganization](../api/connectedorganization-update.md) |Nenhum | Atualizar uma **connectedOrganization**. |
| [Excluir connectedOrganization](../api/connectedorganization-delete.md) |Nenhum | Excluir uma **connectedOrganization**. |
|[Listar internalSponsors](../api/connectedorganization-list-internalsponsors.md) | Conjunto [directoryObject](directoryobject.md) | Recupere uma lista dos **patrocinadores internos de uma connectedOrganization.** |
|[Listar externalSponsors](../api/connectedorganization-list-externalsponsors.md) | Coleção [directoryObject](directoryobject.md) | Recupere uma lista de **patrocinadores externos de uma connectedOrganization.** |
|[Adicionar internalSponsors](../api/connectedorganization-post-internalsponsors.md) | Nenhum | Adicione um usuário ou grupo aos patrocinadores internos de um **connectedOrganization.** |
|[Adicionar externalSponsors](../api/connectedorganization-post-externalsponsors.md) | Nenhum | Adicione um usuário ou grupo aos patrocinadores **externos de um connectedOrganization.** |
|[Remover internalSponsors](../api/connectedorganization-delete-internalsponsors.md) | Nenhum | Remova um usuário ou grupo dos patrocinadores **internos de uma connectedOrganization.** |
|[Remover externalSponsors](../api/connectedorganization-delete-externalsponsors.md) | Nenhum | Remova um usuário ou grupo dos patrocinadores **externos de uma connectedOrganization.** |

## <a name="see-also"></a>Confira também

- [O que é o gerenciamento de direitos do Azure AD?](/azure/active-directory/governance/entitlement-management-overview)
- [subtipos subjectSet](subjectset.md) [singleUser,](singleuser.md) [groupMembers,](groupmembers.md) [connectedOrganizationMembers,](connectedorganizationmembers.md) [requestorManager,](requestormanager.md) [internalSponsors](internalsponsors.md)e [externalSponsors](externalsponsors.md).
- [accessPackageSubject](accesspackagesubject.md) - Usado no [accessPackageAssignment](accesspackageassignment.md) como um usuário de assunto que tem uma atribuição de pacote de acesso.
- [identitySource](identitysource.md) - usado na [connectedOrganization](connectedorganization.md), um dos [azureActiveDirectoryTenant](azureactivedirectorytenant.md), [domainIdentitySource](domainidentitysource.md) ou [externalDomainFederation](externaldomainfederation.md).


