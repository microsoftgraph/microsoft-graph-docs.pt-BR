---
title: Trabalhando com a API Azure AD de gerenciamento de direitos
description: Controlar o acesso a recursos, incluindo grupos, aplicativos e sites Azure AD gerenciamento de direitos
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: conceptualPageType
ms.openlocfilehash: 79f3097f521f40124539314c06973f21b4a8a764
ms.sourcegitcommit: dae41f5828677b993ba89f38c1d1c42d91c0ba02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/29/2022
ms.locfileid: "65133213"
---
# <a name="working-with-the-azure-ad-entitlement-management-api"></a>Trabalhando com a API Azure AD de gerenciamento de direitos

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Azure Active Directory (Azure AD) pode ajudá-lo a gerenciar o acesso a grupos, aplicativos e sites do SharePoint Online para usuários internos, bem como usuários fora da sua organização.

Ao criar pacotes de acesso com as funções que os usuários precisam ter nesses recursos e definir políticas para quem pode solicitar um pacote de acesso e por quanto tempo eles podem ter uma atribuição a um pacote de acesso, você pode controlar o ciclo de vida de acesso para usuários internos e externos.

Os tipos de recursos de gerenciamento de direitos incluem:

- [accessPackage](accesspackage.md): define as coleções de funções de recurso e as políticas de como um ou mais usuários podem obter acesso a esses recursos.
- [accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md): especifica a política pela qual os assuntos podem solicitar ou receber um pacote de acesso por meio de uma atribuição de pacote de acesso.
- [accessPackageAssignmentRequest](accesspackageassignmentrequest.md): criado por um usuário que deseja obter uma atribuição de pacote de acesso.
- [accessPackageAssignment](accesspackageassignment.md): uma atribuição de um pacote de acesso a um assunto específico, por um período de tempo.
- [accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md): indica a função específica do recurso à qual uma entidade foi atribuída por meio de uma atribuição de pacote de acesso.
- [accessPackageCatalog](accesspackagecatalog.md): um contêiner para pacotes de acesso.
- [accessPackageResource](accesspackageresource.md): uma referência a um recurso associado a um catálogo de pacotes de acesso.
- [accessPackageResourceRequest](accesspackageresourcerequest.md): uma solicitação para adicionar um recurso a um catálogo de pacotes de acesso.
- [accessPackageResourceEnvironment](accesspackageresourceenvironment.md): uma referência à localização geográfica do recurso. Aplicável a sites multigeográficos SharePoint Online.
- [connectedOrganization](connectedorganization.md): uma organização conectada para usuários externos que podem solicitar acesso.
- [entitlementManagementSettings](entitlementmanagementsettings.md): configurações em todo o locatário para Azure AD gerenciamento de direitos.
- [aprovação](approval.md): representa as decisões associadas a uma solicitação de pacote de acesso.

Além disso, as atribuições de função para funções específicas do gerenciamento de direitos podem ser gerenciadas por meio de definições de função de gerenciamento [de direitos](unifiedroledefinition.md).

Para obter um tutorial que mostra como usar o gerenciamento de direitos para criar um pacote de recursos que os usuários internos podem solicitar por autoatendimento, consulte Criar um pacote de acesso usando [apIs do Microsoft Graph](/graph/tutorial-access-package-api).

Observe que o recurso de gerenciamento de direitos, incluindo a API, está incluído Azure AD Premium P2. O locatário em que o gerenciamento de direitos está sendo usado deve ter uma assinatura válida de compra ou avaliação Azure AD Premium P2 ou emS E5. Para obter mais informações sobre os requisitos de licença para o recurso de gerenciamento de direitos, consulte [Requisitos de licença de gerenciamento de direitos](/azure/active-directory/governance/entitlement-management-overview#license-requirements).

## <a name="methods"></a>Methods

A tabela a seguir lista os métodos que você pode usar para interagir com recursos relacionados ao gerenciamento de direitos.

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
| [Get](../api/entitlementmanagementsettings-get.md) | [entitlementManagementSettings](entitlementmanagementsettings.md) | Leia as propriedades de **um objeto entitlementManagementSettings** . |
| [Atualizar](../api/entitlementmanagementsettings-update.md) | [entitlementManagementSettings](entitlementmanagementsettings.md) | Atualize as propriedades de **um objeto entitlementManagementSettings** . |
| [Listar accessPackages](../api/entitlementmanagement-list-accesspackages.md) | [Coleção accessPackage](accesspackage.md) | Recupere uma lista de **objetos accessPackage** . |
| [Criar accessPackage](../api/entitlementmanagement-post-accesspackages.md) | [accessPackage](accesspackage.md) | Crie um novo **objeto accessPackage** . |
| [Obter accessPackage](../api/accesspackage-get.md) | [accessPackage](accesspackage.md) | Ler propriedades e relações de um **objeto accessPackage** . |
| [Atualizar accessPackage](../api/accesspackage-update.md)|Nenhum | Atualize as propriedades de um **objeto accesspackage** . |
| [Excluir accessPackage](../api/accesspackage-delete.md) | | **Exclua accessPackage**. |
| [FilterByCurrentUser](../api/accesspackage-filterbycurrentuser.md) | [Coleção accessPackage](accesspackage.md) | Recupere uma lista **de objetos accessPackage** filtrados no usuário conectado. |
| [Listar accessPackageResourceRoleScopes](../api/accesspackage-list-accesspackageresourcerolescopes.md) | [coleção accessPackageResourceRoleScope](accesspackageresourcerolescope.md) | Recupere uma lista de **objetos accessPackageResourceRoleScope** para um pacote de acesso. |
| [Criar accessPackageResourceRoleScope](../api/accesspackage-post-accesspackageresourcerolescopes.md) | | Crie um novo **objeto accessPackageResourceRoleScope** para um pacote de acesso. |
| [Listar incompatibleAccessPackages](../api/accesspackage-list-incompatibleaccesspackages.md) | [Coleção accessPackage](accesspackage.md) | Recupere uma lista dos objetos **accesspackage incompatíveis** para este pacote de acesso. |
| [Adicionar accessPackage a incompatibleAccessPackages](../api/accesspackage-post-incompatibleaccesspackage.md) | Nenhum | Adicione um link para indicar que **outro accesspackage** é incompatível com um pacote de acesso especificado. |
| [Remover accessPackage de incompatibleAccessPackages](../api/accesspackage-delete-incompatibleaccesspackage.md) | Nenhum | Remova um link que indicava que **um accesspackage** era incompatível. |
| [Listar incompatibleGroups](../api/accesspackage-list-incompatiblegroups.md) | Coleção [group](group.md) | Recupere uma lista dos objetos de grupo **incompatíveis** para este pacote de acesso. |
| [Adicionar grupo a incompatibleGroups](../api/accesspackage-post-incompatiblegroup.md) | Nenhum | Adicione um link para indicar que a associação de **um grupo** é incompatível com um pacote de acesso especificado. |
| [Remover grupo de incompatibleGroups](../api/accesspackage-delete-incompatiblegroup.md) | Nenhum | Remova um link que indicava que uma associação **de** grupo era incompatível.|
| [Listar accessPackagesIncompatibleWith](../api/accesspackage-list-accesspackagesincompatiblewith.md) | [Coleção accessPackage](accesspackage.md) | Recupere uma lista dos  **objetos accesspackage** que listam esse pacote de acesso como incompatível. |
| [Listar accessPackageAssignmentPolicies](../api/entitlementmanagement-list-accesspackageassignmentpolicies.md) | [coleção accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) | Recupere uma lista de **objetos accessPackageAssignmentPolicy** . |
| [Criar accessPackageAssignmentPolicy](../api/entitlementmanagement-post-accesspackageassignmentpolicies.md) | [accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md)| Crie um novo **objeto accessPackageAssignmentPolicy** . |
| [Obter accessPackageAssignmentPolicy](../api/accesspackageassignmentpolicy-get.md) | [accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) | Ler propriedades e relações de um **objeto accessPackageAssignmentPolicy** . |
| [Atualizar accessPackageAssignmentPolicy](../api/accesspackageassignmentpolicy-update.md)|[accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) | Atualize as propriedades de **um objeto accessPackageAssignmentPolicy** . |
| [Excluir accessPackageAssignmentPolicy](../api/accesspackageassignmentpolicy-delete.md) | | **Exclua um accessPackageAssignmentPolicy**. |
| [Listar accessPackageAssignmentRequests](../api/entitlementmanagement-list-accesspackageassignmentrequests.md) | [coleção accessPackageAssignmentRequest](accesspackageassignmentrequest.md) | Recupere uma lista de **objetos accessPackageAssignmentRequest** . |
| [Criar accessPackageAssignmentRequest](../api/entitlementmanagement-post-accesspackageassignmentrequests.md) | [accessPackageAssignmentRequest](accesspackageassignmentrequest.md) | Crie um **novo accessPackageAssignmentRequest**. |
| [Obter accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-get.md) | [accessPackageAssignmentRequest](accesspackageassignmentrequest.md) | Ler propriedades e relações de um **objeto accessPackageAssignmentRequest** . |
| [Excluir accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-delete.md) |Nenhum | **Exclua um accessPackageAssignmentRequest**. |
|[FilterByCurrentUser](../api/accesspackageassignmentrequest-filterbycurrentuser.md)|[coleção accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md)|Recupere a lista **de objetos accessPackageAssignmentRequest** filtrados no usuário conectado.|
|[cancel](../api/accesspackageassignmentrequest-cancel.md)|[coleção accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md)|Cancelar um **objeto accessPackageAssignmentRequest** que está em um estado cancelável: `accepted`, `pendingApproval`, `pendingNotBefore`, `pendingApprovalEscalated`.|
| [Listar accessPackageAssignments](../api/entitlementmanagement-list-accesspackageassignments.md) | [coleção accessPackageAssignment](accesspackageassignment.md) | Recupere uma lista de **objetos accessPackageAssignment** . |
|[FilterByCurrentUser](../api/accesspackageassignment-filterbycurrentuser.md)|[coleção accessPackageAssignment](../resources/accesspackageassignment.md)|Recupere a lista de **objetos accessPackageAssignment** filtrados no usuário conectado.|
| [Reprocessar](../api/accesspackageassignment-reprocess.md) | Nenhum | Reavaliar e impor automaticamente as atribuições de um usuário para um pacote de acesso específico.|
| [coleção additionalAccess](../api/accesspackageassignment-additionalaccess.md) [accessPackageAssignment](../resources/accesspackageassignment.md)|Recupere a lista de **objetos accessPackageAssignment** para usuários que têm atribuições a pacotes de acesso incompatíveis.|
| [Listar accessPackageAssignmentResourceRoles](../api/entitlementmanagement-list-accesspackageassignmentresourceroles.md) | [coleção accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md) | Recupere uma lista de **objetos accessPackageAssignmentResourceRole** . |
| [Obter accessPackageAssignmentResourceRole](../api/accesspackageassignmentresourcerole-get.md) | [accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md)  | Recupere um **objeto accessPackageAssignmentResourceRole** . |
| [Listar accessPackageCatalogs](../api/entitlementmanagement-list-accesspackagecatalogs.md) | [coleção accessPackageCatalog](accesspackagecatalog.md) | Recupere uma lista de **objetos accessPackageCatalogs** . |
| [Criar accessPackageCatalog](../api/entitlementmanagement-post-accesspackagecatalogs.md) | [accessPackageCatalog](accesspackagecatalog.md) | Crie um novo **objeto accessPackageCatalog** . |
| [Obter accessPackageCatalog](../api/accesspackagecatalog-get.md) | [accessPackageCatalog](accesspackagecatalog.md) | Ler propriedades e relações de um **objeto accessPackageCatalog** . |
| [Atualizar accessPackageCatalog](../api/accesspackagecatalog-update.md)|Nenhum | Atualize as propriedades de **um objeto accessPackageCatalog** . |
| [Excluir accessPackageCatalog](../api/accesspackagecatalog-delete.md) | | **Exclua um accessPackageCatalog**. |
| [Listar recursos accessPackageCatalog](../api/accesspackagecatalog-list-accesspackageresources.md) | [Coleção accessPackageResource](accesspackageresource.md) | Recupere uma lista de **objetos accessPackageResource** . |
| [Listar funções de recurso accessPackageCatalog](../api/accesspackagecatalog-list-accesspackageresourceroles.md) | [coleção accessPackageResourceRole](accesspackageresourcerole.md) | Recupere uma lista de **objetos accessPackageResourceRole** . |
| [Listar accessPackageResourceRequests](../api/entitlementmanagement-list-accesspackageresourcerequests.md) | [coleção accessPackageResourceRequest](accesspackageresourcerequest.md) | Ler propriedades e relações de **objetos accessPackageResourceRequest** . |
| [Criar accessPackageResourceRequest](../api/entitlementmanagement-post-accesspackageresourcerequests.md) | [accessPackageCatalog](accesspackageresourcerequest.md) | Crie um novo **objeto accessPackageResourceRequest** . |
|[Listar accessPackageResourceEnvironments](../api/entitlementmanagement-list-accesspackageresourceenvironment.md)|[coleção accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md)|Recupere uma lista de [objetos accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) .|
|[Obter accessPackageResourceEnvironment](../api/accesspackageresourceenvironment-get.md)|[accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md)|Leia as propriedades e as relações de um [objeto accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) .|
| [Listar connectedOrganizations](../api/entitlementmanagement-list-connectedorganizations.md) | [coleção connectedOrganization](connectedorganization.md) | Recupere uma lista de **objetos connectedOrganization** . |
| [Criar connectedOrganization](../api/entitlementmanagement-post-connectedorganizations.md) | [connectedOrganization](connectedorganization.md) | Crie um novo **objeto connectedOrganization** . |
| [Obter connectedOrganization](../api/connectedorganization-get.md) | [connectedOrganization](connectedorganization.md) | Ler propriedades e relações de um **objeto connectedOrganization** . |
| [Atualizar connectedOrganization](../api/connectedorganization-update.md) |Nenhum | Atualize **uma connectedOrganization**. |
| [Excluir connectedOrganization](../api/connectedorganization-delete.md) |Nenhum | Exclua **uma connectedOrganization**. |
|[Listar internalSponsors](../api/connectedorganization-list-internalsponsors.md) | Coleção [directoryObject](directoryobject.md) | Recupere uma lista dos **patrocinadores internos de uma connectedOrganization** . |
|[Listar externalSponsors](../api/connectedorganization-list-externalsponsors.md) | Coleção [directoryObject](directoryobject.md) | Recupere uma lista de **patrocinadores externos de uma connectedOrganization** . |
|[Adicionar internalSponsors](../api/connectedorganization-post-internalsponsors.md) | Nenhum | Adicione um usuário ou grupo aos **patrocinadores internos de uma connectedOrganization** . |
|[Adicionar externalSponsors](../api/connectedorganization-post-externalsponsors.md) | Nenhum | Adicione um usuário ou grupo aos **patrocinadores externos de uma connectedOrganization** . |
|[Remover internalSponsors](../api/connectedorganization-delete-internalsponsors.md) | Nenhum | Remova um usuário ou grupo dos **patrocinadores internos de uma connectedOrganization** . |
|[Obter aprovação](../api/approval-get.md) | [aprovação](approval.md) | Recupere as propriedades de um **objeto de** aprovação. |
|[Listar approvalSteps](../api/approval-list-steps.md) | [coleção approvalStep](approvalstep.md) | Liste **os objetos approvalStep** associados a um **objeto de** aprovação. |
|[Obter approvalStep](../api/approvalstep-get.md) | [approvalStep](approvalstep.md) | Recupere as propriedades de um **objeto approvalStep** . |
|[Atualizar approvalStep](../api/approvalstep-update.md) | Nenhum | Aplicar a decisão aprovar ou negar em um **objeto approvalStep** . |


## <a name="types"></a>Tipos

- [requestorSettings](requestorsettings.md), [approvalSettings](approvalsettings.md), [questions](accesspackagequestion.md) e [assignmentReviewSettings](assignmentreviewsettings.md) – usado em [um accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) para especificar quem pode solicitar, quem aprova e quem revisa as solicitações de atribuição de pacote de acesso nessa política.
- [approvalStage](approvalstage.md) – usado em [approvalSettings](approvalsettings.md) para especificar os aprovadores primários, de backup e de escalonamento.
- [approvalStep](approvalstep.md) – usado na [aprovação](approval.md) para distinguir as diferentes etapas de aprovação.
- [subtipos userSet](userset.md) [singleUser](singleuser.md), [groupMembers](groupmembers.md), [connectedOrganizationMembers](connectedorganizationmembers.md), [requestorManager](requestormanager.md), [internalSponsors](internalsponsors.md) e [externalSponsors](externalsponsors.md) - Usado em [requestorSettings](requestorsettings.md), [approvalStage](approvalstage.md), [approvalStep](approvalstep.md) e [assignmentReviewSettings](assignmentreviewsettings.md).
- [accessPackageSubject](accesspackagesubject.md) – usado no [accessPackageAssignment](accesspackageassignment.md) como um usuário da entidade que tem uma atribuição de pacote de acesso.
- [identitySource](identitysource.md) - usado no [connectedOrganization](connectedorganization.md), um de [azureActiveDirectoryTenant](azureactivedirectorytenant.md), [domainIdentitySource](domainidentitysource.md) [ou externalDomainFederation](externaldomainfederation.md).

## <a name="see-also"></a>Confira também

 - [O que Azure AD gerenciamento de direitos?](/azure/active-directory/governance/entitlement-management-overview)



<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Service root",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
