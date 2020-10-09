---
title: Trabalhar com a API de gerenciamento de qualificação do Azure AD
description: Controlar o acesso a recursos, incluindo grupos, aplicativos e sites por meio do gerenciamento de qualificação do Azure AD
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: conceptualPageType
ms.openlocfilehash: f4bb07186ede8949256fba40ad107affaf2889cc
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/09/2020
ms.locfileid: "48400750"
---
# <a name="working-with-the-azure-ad-entitlement-management-api"></a>Trabalhar com a API de gerenciamento de qualificação do Azure AD

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Azure Active Directory (Azure AD) o gerenciamento de direitos pode ajudá-lo a gerenciar o acesso a grupos, aplicativos e sites do SharePoint Online para usuários internos, bem como usuários de fora da sua organização.

Ao criar pacotes do Access com as funções que os usuários precisam ter entre esses recursos e definir políticas para quem pode solicitar um pacote do Access e por quanto tempo eles podem ter uma atribuição a um pacote do Access, você pode governar o ciclo de vida do acesso para usuários internos e externos.

Os tipos de recurso de gerenciamento de direito incluem:

- [accessPackage](accesspackage.md): define as coleções de funções de recurso e as políticas de como um ou mais usuários podem obter acesso a esses recursos.
- [accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md): especifica a política pela qual as entidades podem solicitar ou receber um pacote de acesso por meio de uma atribuição de pacote do Access.
- [accessPackageAssignmentRequest](accesspackageassignmentrequest.md): criado por um usuário que deseja obter uma atribuição de pacote do Access.
- [accessPackageAssignment](accesspackageassignment.md): uma atribuição de um pacote do Access a um assunto específico, por um período de tempo.
- [accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md): indica a função específica do recurso que um assunto foi atribuído por meio de uma atribuição de pacote do Access.
- [accessPackageCatalog](accesspackagecatalog.md): um contêiner para pacotes do Access.
- [accessPackageResourceRequest](accesspackageresourcerequest.md): uma solicitação para adicionar um recurso a um catálogo de pacotes do Access.
- [connectedOrganization](connectedorganization.md): uma organização conectada para usuários externos que podem solicitar acesso.
- [entitlementManagementSettings](entitlementmanagementsettings.md): configurações de todo o locatário para o gerenciamento de qualificação do Azure AD.

Para obter um tutorial que mostra como usar o gerenciamento de qualificação para criar um pacote de recursos que os usuários internos podem solicitar, consulte [Create an Access Package using Microsoft Graph APIs](/graph/tutorial-access-package-api).

Observe que o recurso de gerenciamento de direito, incluindo a API, está incluído no Azure AD Premium P2. O locatário em que o gerenciamento de qualificação está sendo usado deve ter uma assinatura válida de compra ou de avaliação do Azure AD Premium P2 ou EMS e5.

## <a name="methods"></a>Métodos

A tabela a seguir lista os métodos que você pode usar para interagir com recursos relacionados ao gerenciamento de direitos.

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
| [Get](../api/entitlementmanagementsettings-get.md) | [entitlementManagementSettings](entitlementmanagementsettings.md) | Ler as propriedades de um objeto **entitlementManagementSettings** . |
| [Update](../api/entitlementmanagementsettings-update.md) | [entitlementManagementSettings](entitlementmanagementsettings.md) | Atualiza as propriedades de um objeto **entitlementManagementSettings** . |
| [Listar accessPackages](../api/accesspackage-list.md) | coleção [accessPackage](accesspackage.md) | Recupere uma lista de objetos **accessPackage** . |
| [Criar accessPackage](../api/accesspackage-post.md) | [accessPackage](accesspackage.md) | Criar um novo objeto **accessPackage** . |
| [Obter accessPackage](../api/accesspackage-get.md) | [accessPackage](accesspackage.md) | Ler propriedades e relações de um objeto **accessPackage** . |
| [Atualizar accessPackage](../api/accesspackage-update.md)|Nenhum | Atualiza as propriedades de um objeto **accesspackage** . |
| [Excluir accessPackage](../api/accesspackage-delete.md) | | Exclua **accessPackage**. |
| [Listar accessPackageResourceRoleScopes](../api/accesspackage-list-accesspackageresourcerolescopes.md) | coleção [accessPackageResourceRoleScope](accesspackageresourcerolescope.md) | Recupere uma lista de objetos **accessPackageResourceRoleScope** para um pacote do Access. |
| [Criar accessPackageResourceRoleScope](../api/accesspackage-post-accesspackageresourcerolescopes.md) | | Criar um novo objeto **accessPackageResourceRoleScope** para um pacote do Access. |
| [Listar accessPackageAssignmentPolicies](../api/accesspackageassignmentpolicy-list.md) | coleção [accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) | Recupere uma lista de objetos **accessPackageAssignmentPolicy** . |
| [Criar accessPackageAssignmentPolicy](../api/accesspackageassignmentpolicy-post.md) | [accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md)| Criar um novo objeto **accessPackageAssignmentPolicy** . |
| [Obter accessPackageAssignmentPolicy](../api/accesspackageassignmentpolicy-get.md) | [accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) | Ler propriedades e relações de um objeto **accessPackageAssignmentPolicy** . |
| [Atualizar accessPackageAssignmentPolicy](../api/accesspackageassignmentpolicy-update.md)|[accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) | Atualiza as propriedades de um objeto **accessPackageAssignmentPolicy** . |
| [Excluir accessPackageAssignmentPolicy](../api/accesspackageassignmentpolicy-delete.md) | | Excluir um **accessPackageAssignmentPolicy**. |
| [Listar accessPackageAssignmentRequests](../api/accesspackageassignmentrequest-list.md) | coleção [accessPackageAssignmentRequest](accesspackageassignmentrequest.md) | Recupere uma lista de objetos **accessPackageAssignmentRequest** . |
| [Criar accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md) | [accessPackageAssignmentRequest](accesspackageassignmentrequest.md) | Criar um novo **accessPackageAssignmentRequest**. |
| [Obter accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-get.md) | [accessPackageAssignmentRequest](accesspackageassignmentrequest.md) | Ler propriedades e relações de um objeto **accessPackageAssignmentRequest** . |
| [Listar accessPackageAssignments](../api/accesspackageassignment-list.md) | coleção [accessPackageAssignment](accesspackageassignment.md) | Recupere uma lista de objetos **accessPackageAssignment** . |
| [Listar accessPackageAssignmentResourceRoles](../api/accesspackageassignmentresourcerole-list.md) | coleção [accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md) | Recupere uma lista de objetos **accessPackageAssignmentResourceRole** . |
| [Obter accessPackageAssignmentResourceRole](../api/accesspackageassignmentresourcerole-get.md) | [accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md)  | Recupere um objeto **accessPackageAssignmentResourceRole** . |
| [Listar accessPackageCatalogs](../api/accesspackagecatalog-list.md) | coleção [accessPackageCatalog](accesspackagecatalog.md) | Recupere uma lista de objetos **accessPackageCatalogs** . |
| [Criar accessPackageCatalog](../api/accesspackagecatalog-post.md) | [accessPackageCatalog](accesspackagecatalog.md) | Criar um novo objeto **accessPackageCatalog** . |
| [Obter accessPackageCatalog](../api/accesspackagecatalog-get.md) | [accessPackageCatalog](accesspackagecatalog.md) | Ler propriedades e relações de um objeto **accessPackageCatalog** . |
| [Atualizar accessPackageCatalog](../api/accesspackagecatalog-update.md)|Nenhum | Atualiza as propriedades de um objeto **accessPackageCatalog** . |
| [Excluir accessPackageCatalog](../api/accesspackagecatalog-delete.md) | | Excluir um **accessPackageCatalog**. |
| [Listar recursos do accessPackageCatalog](../api/accesspackagecatalog-list-accesspackageresources.md) | coleção [accessPackageResource](accesspackageresource.md) | Recupere uma lista de objetos **accessPackageResource** . |
| [Listar funções de recurso accessPackageCatalog](../api/accesspackagecatalog-list-accesspackageresourceroles.md) | coleção [accessPackageResourceRole](accesspackageresourcerole.md) | Recupere uma lista de objetos **accessPackageResourceRole** . |
| [Listar accessPackageResourceRequests](../api/accesspackageresourcerequest-list.md) | coleção [accessPackageResourceRequest](accesspackageresourcerequest.md) | Ler propriedades e relações de objetos **accessPackageResourceRequest** . |
| [Criar accessPackageResourceRequest](../api/accesspackageresourcerequest-post.md) | [accessPackageCatalog](accesspackageresourcerequest.md) | Criar um novo objeto **accessPackageResourceRequest** . |
| [Listar connectedOrganizations](../api/connectedorganization-list.md) | coleção [connectedOrganization](connectedorganization.md) | Recupere uma lista de objetos **connectedOrganization** . |
| [Criar connectedOrganization](../api/connectedorganization-post.md) | [connectedOrganization](connectedorganization.md) | Criar um novo objeto **connectedOrganization** . |
| [Obter connectedOrganization](../api/connectedorganization-get.md) | [connectedOrganization](connectedorganization.md) | Ler propriedades e relações de um objeto **connectedOrganization** . |
| [Atualizar connectedOrganization](../api/connectedorganization-update.md) |Nenhum | Atualizar um **connectedOrganization**. |
| [Excluir connectedOrganization](../api/connectedorganization-delete.md) |Nenhum | Excluir um **connectedOrganization**. |
|[Listar internalSponsors](../api/connectedorganization-list-internalsponsors.md) | Coleção [directoryObject](directoryobject.md) | Recupere uma lista de patrocinadores internos de um **connectedOrganization** . |
|[Listar externalSponsors](../api/connectedorganization-list-externalsponsors.md) | Coleção [directoryObject](directoryobject.md) | Recupere uma lista de patrocinadores externos de um **connectedOrganization** . |
|[Adicionar internalSponsors](../api/connectedorganization-post-internalsponsors.md) | Nenhum | Adicionar um usuário ou grupo aos patrocinadores internos de um **connectedOrganization** . |
|[Adicionar externalSponsors](../api/connectedorganization-post-externalsponsors.md) | Nenhum | Adicionar um usuário ou grupo aos patrocinadores externos de um **connectedOrganization** . |
|[Remover internalSponsors](../api/connectedorganization-delete-internalsponsors.md) | Nenhum | Remover um usuário ou grupo dos patrocinadores internos de um **connectedOrganization** . |
|[Remover externalSponsors](../api/connectedorganization-delete-externalsponsors.md) | Nenhum | Remover um usuário ou grupo dos patrocinadores externos de um **connectedOrganization** . |

## <a name="types"></a>Tipos

- [requestorSettings](requestorsettings.md), [approvalSettings](approvalsettings.md) e [AssignmentReviewSettings](assignmentreviewsettings.md) -usados em um [accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) para especificar quem pode solicitar, quem aprova e quem revisa as solicitações de atribuição de pacote de acesso nessa política.
- [approvalStage](approvalstage.md) -usado no [approvalSettings](approvalsettings.md) para especificar os aprovadores primário, de backup e de escalonamento.
- [userset](userset.md) subtipos [únicousuário](singleuser.md), [groupMembers](groupmembers.md), [connectedOrganizationMembers](connectedorganizationmembers.md), [requestorManager](requestormanager.md), [internalSponsors](internalsponsors.md)e [externalSponsors](externalsponsors.md) -usados em [requestorSettings](requestorsettings.md), [approvalStage](approvalstage.md) e [assignmentReviewSettings](assignmentreviewsettings.md).
- [accessPackageSubject](accesspackagesubject.md) -usado no [accessPackageAssignment](accesspackageassignment.md) como um usuário do requerente que tem uma atribuição de pacote do Access.
- [identityr](identitysource.md) -usado no [connectedOrganization](connectedorganization.md), um de [azureActiveDirectoryTenant](azureactivedirectorytenant.md), [domainIdentitySource](domainidentitysource.md) ou [externalDomainFederation](externaldomainfederation.md).

## <a name="see-also"></a>Confira também

 - [O que é gerenciamento de qualificação do AD do Azure?](/azure/active-directory/governance/entitlement-management-overview)



<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Service root",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->