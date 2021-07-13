---
title: Trabalhando com a API de gerenciamento de direitos do Azure AD
description: Governe o acesso a recursos, incluindo grupos, aplicativos e sites por meio do gerenciamento de direitos do Azure AD
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: conceptualPageType
ms.openlocfilehash: c75c88c4f7fd2d35eb6e214bbe3479abdac6b4da
ms.sourcegitcommit: 8b23038be1141d7f22eb61de6aafdb16d4f9c826
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401467"
---
# <a name="working-with-the-azure-ad-entitlement-management-api"></a>Trabalhando com a API de gerenciamento de direitos do Azure AD

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Azure Active Directory (Azure AD) gerenciamento de direitos pode ajudá-lo a gerenciar o acesso a grupos, aplicativos e sites SharePoint Online para usuários internos, bem como usuários fora da sua organização.

Ao criar pacotes de acesso com as funções que os usuários precisam ter nesses recursos e definir políticas para quem pode solicitar um pacote de acesso e por quanto tempo eles podem ter uma atribuição para um pacote de acesso, você pode reger o ciclo de vida do acesso para usuários internos e externos.

Os tipos de recursos de gerenciamento de direitos incluem:

- [accessPackage](accesspackage.md): define as coleções de funções de recurso e as políticas de como um ou mais usuários podem obter acesso a esses recursos.
- [accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md): especifica a política pela qual os titulares podem solicitar ou ter um pacote de acesso atribuído por meio de uma atribuição de pacote de acesso.
- [accessPackageAssignmentRequest](accesspackageassignmentrequest.md): Criado por um usuário que deseja obter uma atribuição de pacote de acesso.
- [accessPackageAssignment](accesspackageassignment.md): Uma atribuição de um pacote de acesso a um assunto específico, por um período de tempo.
- [accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md): Indica a função específica do recurso que um assunto foi atribuído por meio de uma atribuição de pacote de acesso.
- [accessPackageCatalog](accesspackagecatalog.md): um contêiner para pacotes de acesso.
- [accessPackageResourceRequest](accesspackageresourcerequest.md): Uma solicitação para adicionar um recurso a um catálogo de pacotes de acesso.
- [accessPackageResourceEnvironment](accesspackageresourceenvironment.md): uma referência à localização geográfica do recurso. Aplicável a sites multi-SharePoint Online.
- [connectedOrganization](connectedorganization.md): uma organização conectada para usuários externos que podem solicitar acesso.
- [entitlementManagementSettings](entitlementmanagementsettings.md): configurações de todo o locatário para o gerenciamento de direitos do Azure AD.
- [aprovação](approval.md): representa as decisões associadas a uma solicitação de pacote de acesso.

Além disso, as atribuições de função para funções específicas de gerenciamento de direitos podem ser gerenciadas por meio de definições de função de gerenciamento de [direitos.](unifiedroledefinition.md)

For a tutorial that shows you how to use entitlement management to create a package of resources that internal users can self-service request, see [Create an access package using Microsoft Graph APIs](/graph/tutorial-access-package-api).

Observe que o recurso de gerenciamento de direitos, incluindo a API, está incluído Azure AD Premium P2. O locatário em que o gerenciamento de direitos está sendo usado deve ter uma assinatura de compra ou avaliação válida Azure AD Premium P2 ou EMS E5.

## <a name="methods"></a>Métodos

A tabela a seguir lista os métodos que você pode usar para interagir com recursos relacionados ao gerenciamento de direitos.

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
| [Get](../api/entitlementmanagementsettings-get.md) | [entitlementManagementSettings](entitlementmanagementsettings.md) | Leia as propriedades de **um objeto entitlementManagementSettings.** |
| [Atualizar](../api/entitlementmanagementsettings-update.md) | [entitlementManagementSettings](entitlementmanagementsettings.md) | Atualize as propriedades de **um objeto entitlementManagementSettings.** |
| [Listar accessPackages](../api/accesspackage-list.md) | [Coleção accessPackage](accesspackage.md) | Recupere uma lista de **objetos accessPackage.** |
| [Criar accessPackage](../api/accesspackage-post.md) | [accessPackage](accesspackage.md) | Crie um novo **objeto accessPackage.** |
| [Obter accessPackage](../api/accesspackage-get.md) | [accessPackage](accesspackage.md) | Ler propriedades e relações de um **objeto accessPackage.** |
| [Atualizar accessPackage](../api/accesspackage-update.md)|Nenhum | Atualize as propriedades de um **objeto accesspackage.** |
| [Excluir accessPackage](../api/accesspackage-delete.md) | | Excluir **accessPackage**. |
| [FilterByCurrentUser](../api/accesspackage-filterbycurrentuser.md) | [Coleção accessPackage](accesspackage.md) | Recupere uma lista de **objetos accessPackage** filtrados no usuário de entrada. |
| [Listar accessPackageResourceRoleScopes](../api/accesspackage-list-accesspackageresourcerolescopes.md) | [Coleção accessPackageResourceRoleScope](accesspackageresourcerolescope.md) | Recupere uma lista de **objetos accessPackageResourceRoleScope** para um pacote de acesso. |
| [Criar accessPackageResourceRoleScope](../api/accesspackage-post-accesspackageresourcerolescopes.md) | | Crie um novo **objeto accessPackageResourceRoleScope** para um pacote de acesso. |
| [Listar incompatívelAccessPackages](../api/accesspackage-list-incompatibleaccesspackages.md) | [Coleção accessPackage](accesspackage.md) | Recupere uma lista dos objetos **accesspackage** incompatíveis para este pacote de acesso. |
| [Adicionar accessPackage a incompatibleAccessPackages](../api/accesspackage-post-incompatibleaccesspackage.md) | Nenhum | Adicione um link para indicar que outro **pacote de acessos** é incompatível com um pacote de acesso especificado. |
| [Remover accessPackage de incompatívelAccessPackages](../api/accesspackage-delete-incompatibleaccesspackage.md) | Nenhum | Remover um link que indicava que um **pacote de acesso** era incompatível. |
| [Listar incompatibleGroups](../api/accesspackage-list-incompatiblegroups.md) | Coleção [group](group.md) | Recupere uma lista dos objetos **de** grupo incompatíveis para este pacote de acesso. |
| [Adicionar grupo a incompatibleGroups](../api/accesspackage-post-incompatiblegroup.md) | Nenhum | Adicione um link para indicar que a associação de um **grupo** é incompatível com um pacote de acesso especificado. |
| [Remover grupo de incompatibleGroups](../api/accesspackage-delete-incompatiblegroup.md) | Nenhum | Remover um link que indicava que uma associação **ao** grupo era incompatível.|
| [Listar accessPackagesIncompatibleWith](../api/accesspackage-list-accesspackagesincompatiblewith.md) | [Coleção accessPackage](accesspackage.md) | Recupere uma lista dos  **objetos accesspackage que** listam esse pacote de acesso como incompatível. |
| [Listar accessPackageAssignmentPolicies](../api/accesspackageassignmentpolicy-list.md) | [coleção accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) | Recupere uma lista de **objetos accessPackageAssignmentPolicy.** |
| [Criar accessPackageAssignmentPolicy](../api/accesspackageassignmentpolicy-post.md) | [accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md)| Crie um novo **objeto accessPackageAssignmentPolicy.** |
| [Obter accessPackageAssignmentPolicy](../api/accesspackageassignmentpolicy-get.md) | [accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) | Ler propriedades e relações de um **objeto accessPackageAssignmentPolicy.** |
| [Atualizar accessPackageAssignmentPolicy](../api/accesspackageassignmentpolicy-update.md)|[accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) | Atualize as propriedades de **um objeto accessPackageAssignmentPolicy.** |
| [Excluir accessPackageAssignmentPolicy](../api/accesspackageassignmentpolicy-delete.md) | | Excluir um **accessPackageAssignmentPolicy**. |
| [Listar accessPackageAssignmentRequests](../api/accesspackageassignmentrequest-list.md) | [coleção accessPackageAssignmentRequest](accesspackageassignmentrequest.md) | Recupere uma lista de **objetos accessPackageAssignmentRequest.** |
| [Criar accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md) | [accessPackageAssignmentRequest](accesspackageassignmentrequest.md) | Crie um novo **accessPackageAssignmentRequest**. |
| [Obter accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-get.md) | [accessPackageAssignmentRequest](accesspackageassignmentrequest.md) | Leia propriedades e relações de um **objeto accessPackageAssignmentRequest.** |
|[FilterByCurrentUser](../api/accesspackageassignmentrequest-filterbycurrentuser.md)|[coleção accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md)|Recupere a lista de **objetos accessPackageAssignmentRequest** filtrados no usuário de entrada.|
|[cancel](../api/accesspackageassignmentrequest-cancel.md)|[coleção accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md)|Cancele **um objeto accessPackageAssignmentRequest** que está em estado cancelável: `accepted` , , , `pendingApproval` `pendingNotBefore` `pendingApprovalEscalated` .|
| [Listar accessPackageAssignments](../api/accesspackageassignment-list.md) | [Coleção accessPackageAssignment](accesspackageassignment.md) | Recupere uma lista de **objetos accessPackageAssignment.** |
|[FilterByCurrentUser](../api/accesspackageassignment-filterbycurrentuser.md)|[Coleção accessPackageAssignment](../resources/accesspackageassignment.md)|Recupere a lista de **objetos accessPackageAssignment** filtrados no usuário de entrada.|
| [Listar accessPackageAssignmentResourceRoles](../api/accesspackageassignmentresourcerole-list.md) | [Coleção accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md) | Recupere uma lista de **objetos accessPackageAssignmentResourceRole.** |
| [Obter accessPackageAssignmentResourceRole](../api/accesspackageassignmentresourcerole-get.md) | [accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md)  | Recupere um **objeto accessPackageAssignmentResourceRole.** |
| [Listar accessPackageCatalogs](../api/accesspackagecatalog-list.md) | [Coleção accessPackageCatalog](accesspackagecatalog.md) | Recupere uma lista de **objetos accessPackageCatalogs.** |
| [Criar accessPackageCatalog](../api/accesspackagecatalog-post.md) | [accessPackageCatalog](accesspackagecatalog.md) | Crie um novo **objeto accessPackageCatalog.** |
| [Obter accessPackageCatalog](../api/accesspackagecatalog-get.md) | [accessPackageCatalog](accesspackagecatalog.md) | Ler propriedades e relações de um **objeto accessPackageCatalog.** |
| [Atualizar accessPackageCatalog](../api/accesspackagecatalog-update.md)|Nenhum | Atualize as propriedades de um **objeto accessPackageCatalog.** |
| [Excluir accessPackageCatalog](../api/accesspackagecatalog-delete.md) | | Excluir um **accessPackageCatalog**. |
| [Listar recursos do accessPackageCatalog](../api/accesspackagecatalog-list-accesspackageresources.md) | [Coleção accessPackageResource](accesspackageresource.md) | Recupere uma lista de **objetos accessPackageResource.** |
| [Listar funções de recurso accessPackageCatalog](../api/accesspackagecatalog-list-accesspackageresourceroles.md) | [Coleção accessPackageResourceRole](accesspackageresourcerole.md) | Recupere uma lista de **objetos accessPackageResourceRole.** |
| [Listar accessPackageResourceRequests](../api/accesspackageresourcerequest-list.md) | [Coleção accessPackageResourceRequest](accesspackageresourcerequest.md) | Ler propriedades e relações de **objetos accessPackageResourceRequest.** |
| [Criar accessPackageResourceRequest](../api/accesspackageresourcerequest-post.md) | [accessPackageCatalog](accesspackageresourcerequest.md) | Crie um novo **objeto accessPackageResourceRequest.** |
|[Listar accessPackageResourceEnvironments](../api/accesspackageresourceenvironment-list.md)|[coleção accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md)|Recupere uma lista de [objetos accessPackageResourceEnvironment.](../resources/accesspackageresourceenvironment.md)|
|[Obter accessPackageResourceEnvironment](../api/accesspackageresourceenvironment-get.md)|[accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md)|Leia as propriedades e as relações de um [objeto accessPackageResourceEnvironment.](../resources/accesspackageresourceenvironment.md)|
| [Listar connectedOrganizations](../api/connectedorganization-list.md) | [Coleção connectedOrganization](connectedorganization.md) | Recupere uma lista de **objetos connectedOrganization.** |
| [Criar connectedOrganization](../api/connectedorganization-post.md) | [connectedOrganization](connectedorganization.md) | Crie um novo **objeto connectedOrganization.** |
| [Obter connectedOrganization](../api/connectedorganization-get.md) | [connectedOrganization](connectedorganization.md) | Leia propriedades e relações de um **objeto connectedOrganization.** |
| [Atualizar connectedOrganization](../api/connectedorganization-update.md) |Nenhum | Atualizar uma **connectedOrganization**. |
| [Excluir connectedOrganization](../api/connectedorganization-delete.md) |Nenhum | Excluir uma **connectedOrganization**. |
|[Listar internalSponsors](../api/connectedorganization-list-internalsponsors.md) | Coleção [directoryObject](directoryobject.md) | Recupere uma lista dos **patrocinadores internos de uma connectedOrganization.** |
|[Listar externalSponsors](../api/connectedorganization-list-externalsponsors.md) | Coleção [directoryObject](directoryobject.md) | Recupere uma lista de **patrocinadores externos de uma connectedOrganization.** |
|[Adicionar internalSponsors](../api/connectedorganization-post-internalsponsors.md) | Nenhum | Adicione um usuário ou grupo aos patrocinadores internos de um **connectedOrganization.** |
|[Adicionar externalSponsors](../api/connectedorganization-post-externalsponsors.md) | Nenhum | Adicione um usuário ou grupo aos patrocinadores **externos de um connectedOrganization.** |
|[Remover internalSponsors](../api/connectedorganization-delete-internalsponsors.md) | Nenhum | Remova um usuário ou grupo dos patrocinadores **internos de uma connectedOrganization.** |
|[Obter aprovação](../api/approval-get.md) | [aprovação](approval.md) | Recupere as propriedades de um **objeto de aprovação.** |
|[Aprovação de listaSteps](../api/approval-list-steps.md) | [Coleção approvalStep](approvalstep.md) | Listar **os objetos approvalStep** associados a um **objeto de** aprovação. |
|[Obter approvalStep](../api/approvalstep-get.md) | [approvalStep](approvalstep.md) | Recupere as propriedades de um **objeto approvalStep.** |
|[Atualizar approvalStep](../api/approvalstep-update.md) | Nenhum | Aplicar aprovar ou negar decisão em um **objeto approvalStep.** |


## <a name="types"></a>Tipos

- [requestorSettings](requestorsettings.md), [approvalSettings](approvalsettings.md) [,](accesspackagequestion.md) questions and [assignmentReviewSettings](assignmentreviewsettings.md) - Usado em [um accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) para especificar quem pode solicitar, quem aprova e quem revisa solicitações de atribuição de pacote de acesso nessa política.
- [approvalStage](approvalstage.md) - Usado nas [approvalSettings](approvalsettings.md) para especificar os aprovadores primários, de backup e de escalonamento.
- [approvalStep](approvalstep.md) - Usado na [aprovação](approval.md) para distinguir as diferentes etapas de aprovação.
- [userSet](userset.md) subtypes [singleUser](singleuser.md), [groupMembers](groupmembers.md), [connectedOrganizationMembers](connectedorganizationmembers.md), [requestorManager](requestormanager.md), [internalSponsors](internalsponsors.md)e [externalSponsors](externalsponsors.md) - Usado em [requestorSettings](requestorsettings.md), [approvalStage,](approvalstage.md) [approvalStep](approvalstep.md) e [assignmentReviewSettings](assignmentreviewsettings.md).
- [accessPackageSubject](accesspackagesubject.md) - Usado no [accessPackageAssignment](accesspackageassignment.md) como um usuário de assunto que tem uma atribuição de pacote de acesso.
- [identitySource](identitysource.md) - usado na [connectedOrganization](connectedorganization.md), um dos [azureActiveDirectoryTenant](azureactivedirectorytenant.md), [domainIdentitySource](domainidentitysource.md) ou [externalDomainFederation](externaldomainfederation.md).

## <a name="see-also"></a>Confira também

 - [O que é o gerenciamento de direitos do Azure AD?](/azure/active-directory/governance/entitlement-management-overview)



<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Service root",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
