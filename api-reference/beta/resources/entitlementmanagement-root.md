---
title: Trabalhar com a API de gerenciamento de direitos do Azure AD
description: Controle o acesso a recursos, incluindo grupos, aplicativos e sites por meio do gerenciamento de direitos do Azure AD
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: conceptualPageType
ms.openlocfilehash: d2363e60a0eb99388d3da36264802f87bc12ee93
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131527"
---
# <a name="working-with-the-azure-ad-entitlement-management-api"></a>Trabalhar com a API de gerenciamento de direitos do Azure AD

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O gerenciamento de direitos do Azure Active Directory (Azure AD) pode ajudá-lo a gerenciar o acesso a grupos, aplicativos e sites do SharePoint Online para usuários internos, bem como usuários de fora da sua organização.

Criando pacotes de acesso com as funções que os usuários precisam ter nesses recursos e definindo políticas para quem pode solicitar um pacote de acesso e por quanto tempo eles podem ter uma atribuição a um pacote de acesso, você pode reger o ciclo de vida de acesso para usuários internos e externos.

Os tipos de recursos de gerenciamento de direitos incluem:

- [accessPackage](accesspackage.md): define as coleções de funções de recurso e as políticas de como um ou mais usuários podem obter acesso a esses recursos.
- [accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md): especifica a política pela qual os assuntos podem solicitar ou ser atribuídos a um pacote de acesso por meio de uma atribuição de pacote de acesso.
- [accessPackageAssignmentRequest](accesspackageassignmentrequest.md): criado por um usuário que deseja obter uma atribuição de pacote de acesso.
- [accessPackageAssignment](accesspackageassignment.md): uma atribuição de um pacote de acesso a um assunto específico, por um período de tempo.
- [accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md): indica a função específica do recurso à qual um assunto foi atribuído por meio de uma atribuição de pacote de acesso.
- [accessPackageCatalog](accesspackagecatalog.md): um contêiner para pacotes de acesso.
- [accessPackageResourceRequest](accesspackageresourcerequest.md): uma solicitação para adicionar um recurso a um catálogo de pacotes de acesso.
- [accessPackageResourceEnvironment:](accesspackageresourceenvironment.md)uma referência à localização geográfica do recurso. Aplicável a sites multi-geo do SharePoint Online.
- [connectedOrganization](connectedorganization.md): uma organização conectada para usuários externos que podem solicitar acesso.
- [entitlementManagementSettings](entitlementmanagementsettings.md): configurações de todo o locatário para o gerenciamento de direitos do Azure AD.

For a tutorial that shows you how to use entitlement management to create a package of resources that internal users can self-service request, see [Create an access package using Microsoft Graph APIs](/graph/tutorial-access-package-api).

Observe que o recurso de gerenciamento de direitos, incluindo a API, está incluído no Azure AD Premium P2. O locatário em que o gerenciamento de direitos está sendo usado deve ter uma assinatura válida adquirida ou de avaliação do Azure AD Premium P2 ou EMS E5.

## <a name="methods"></a>Métodos

A tabela a seguir lista os métodos que você pode usar para interagir com recursos relacionados ao gerenciamento de direitos.

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
| [Get](../api/entitlementmanagementsettings-get.md) | [entitlementManagementSettings](entitlementmanagementsettings.md) | Leia as propriedades de um **objeto entitlementManagementSettings** . |
| [Update](../api/entitlementmanagementsettings-update.md) | [entitlementManagementSettings](entitlementmanagementsettings.md) | Atualizar as propriedades de um **objeto entitlementManagementSettings.** |
| [Listar accessPackages](../api/accesspackage-list.md) | [coleção accessPackage](accesspackage.md) | Recupere uma lista de **objetos accessPackage.** |
| [Criar accessPackage](../api/accesspackage-post.md) | [accessPackage](accesspackage.md) | Criar um novo **objeto accessPackage.** |
| [Obter accessPackage](../api/accesspackage-get.md) | [accessPackage](accesspackage.md) | Leia as propriedades e as relações de um **objeto accessPackage.** |
| [Atualizar accessPackage](../api/accesspackage-update.md)|Nenhuma | Atualizar as propriedades de um **objeto accesspackage.** |
| [Excluir accessPackage](../api/accesspackage-delete.md) | | Excluir **accessPackage**. |
| [Listar accessPackageResourceRoleScopes](../api/accesspackage-list-accesspackageresourcerolescopes.md) | [Coleção accessPackageResourceRoleScope](accesspackageresourcerolescope.md) | Recupere uma lista de **objetos accessPackageResourceRoleScope** para um pacote de acesso. |
| [Criar accessPackageResourceRoleScope](../api/accesspackage-post-accesspackageresourcerolescopes.md) | | Crie um novo **objeto accessPackageResourceRoleScope** para um pacote de acesso. |
| [Listar accessPackageAssignmentPolicies](../api/accesspackageassignmentpolicy-list.md) | [coleção accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) | Recupere uma lista de **objetos accessPackageAssignmentPolicy.** |
| [Criar accessPackageAssignmentPolicy](../api/accesspackageassignmentpolicy-post.md) | [accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md)| Criar um novo **objeto accessPackageAssignmentPolicy.** |
| [Acessar AccessPackageAssignmentPolicy](../api/accesspackageassignmentpolicy-get.md) | [accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) | Ler propriedades e relações de um **objeto accessPackageAssignmentPolicy.** |
| [Atualizar accessPackageAssignmentPolicy](../api/accesspackageassignmentpolicy-update.md)|[accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) | Atualizar as propriedades de um **objeto accessPackageAssignmentPolicy.** |
| [Excluir accessPackageAssignmentPolicy](../api/accesspackageassignmentpolicy-delete.md) | | **Exclua um accessPackageAssignmentPolicy**. |
| [Listar accessPackageAssignmentRequests](../api/accesspackageassignmentrequest-list.md) | [coleção accessPackageAssignmentRequest](accesspackageassignmentrequest.md) | Recupere uma lista de **objetos accessPackageAssignmentRequest.** |
| [Criar accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md) | [accessPackageAssignmentRequest](accesspackageassignmentrequest.md) | Crie um novo **accessPackageAssignmentRequest**. |
| [Acessar AccessPackageAssignmentRequest](../api/accesspackageassignmentrequest-get.md) | [accessPackageAssignmentRequest](accesspackageassignmentrequest.md) | Ler propriedades e relações de um **objeto accessPackageAssignmentRequest.** |
| [Listar accessPackageAssignments](../api/accesspackageassignment-list.md) | [Coleção accessPackageAssignment](accesspackageassignment.md) | Recupere uma lista de **objetos accessPackageAssignment.** |
| [Listar accessPackageAssignmentResourceRoles](../api/accesspackageassignmentresourcerole-list.md) | [Coleção accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md) | Recupere uma lista de **objetos accessPackageAssignmentResourceRole.** |
| [Acessar AccessPackageAssignmentResourceRole](../api/accesspackageassignmentresourcerole-get.md) | [accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md)  | Recupere um **objeto accessPackageAssignmentResourceRole.** |
| [Listar accessPackageCatalogs](../api/accesspackagecatalog-list.md) | [coleção accessPackageCatalog](accesspackagecatalog.md) | Recupere uma lista de **objetos accessPackageCatalogs.** |
| [Criar accessPackageCatalog](../api/accesspackagecatalog-post.md) | [accessPackageCatalog](accesspackagecatalog.md) | Criar um novo **objeto accessPackageCatalog.** |
| [Obter accessPackageCatalog](../api/accesspackagecatalog-get.md) | [accessPackageCatalog](accesspackagecatalog.md) | Ler propriedades e relações de um **objeto accessPackageCatalog.** |
| [Atualizar accessPackageCatalog](../api/accesspackagecatalog-update.md)|Nenhuma | Atualizar as propriedades de um **objeto accessPackageCatalog.** |
| [Excluir accessPackageCatalog](../api/accesspackagecatalog-delete.md) | | **Exclua um accessPackageCatalog**. |
| [Listar recursos accessPackageCatalog](../api/accesspackagecatalog-list-accesspackageresources.md) | [Coleção accessPackageResource](accesspackageresource.md) | Recupere uma lista de **objetos accessPackageResource.** |
| [Listar funções de recurso accessPackageCatalog](../api/accesspackagecatalog-list-accesspackageresourceroles.md) | [Coleção accessPackageResourceRole](accesspackageresourcerole.md) | Recupere uma lista de **objetos accessPackageResourceRole.** |
| [Listar accessPackageResourceRequests](../api/accesspackageresourcerequest-list.md) | [coleção accessPackageResourceRequest](accesspackageresourcerequest.md) | Leia as propriedades e as relações dos **objetos accessPackageResourceRequest.** |
| [Criar accessPackageResourceRequest](../api/accesspackageresourcerequest-post.md) | [accessPackageCatalog](accesspackageresourcerequest.md) | Criar um novo **objeto accessPackageResourceRequest.** |
|[Listar accessPackageResourceEnvironments](../api/accesspackageresourceenvironment-list.md)|[Coleção accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md)|Recupere uma lista de [objetos accessPackageResourceEnvironment.](../resources/accesspackageresourceenvironment.md)|
|[Acessar AccessPackageResourceEnvironment](../api/accesspackageresourceenvironment-get.md)|[accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md)|Leia as propriedades e os relacionamentos de um [objeto accessPackageResourceEnvironment.](../resources/accesspackageresourceenvironment.md)|
| [Listar connectedOrganizations](../api/connectedorganization-list.md) | [Coleção connectedOrganization](connectedorganization.md) | Recupere uma lista de **objetos connectedOrganization.** |
| [Criar connectedOrganization](../api/connectedorganization-post.md) | [connectedOrganization](connectedorganization.md) | Crie um novo **objeto connectedOrganization.** |
| [Obter connectedOrganization](../api/connectedorganization-get.md) | [connectedOrganization](connectedorganization.md) | Leia as propriedades e as relações de um **objeto connectedOrganization.** |
| [Atualizar connectedOrganization](../api/connectedorganization-update.md) |Nenhuma | Atualizar uma **connectedOrganization**. |
| [Excluir connectedOrganization](../api/connectedorganization-delete.md) |Nenhuma | Exclua **uma connectedOrganization**. |
|[Listar internalSponsors](../api/connectedorganization-list-internalsponsors.md) | Coleção [directoryObject](directoryobject.md) | Recupere uma lista de **patrocinadores internos de** uma organização conectada. |
|[Listar externalSponsors](../api/connectedorganization-list-externalsponsors.md) | Coleção [directoryObject](directoryobject.md) | Recupere uma lista de **patrocinadores externos de** uma organização conectada. |
|[Adicionar internalSponsors](../api/connectedorganization-post-internalsponsors.md) | Nenhuma | Adicione um usuário ou grupo aos **patrocinadores internos de** uma organização conectada. |
|[Adicionar externalSponsors](../api/connectedorganization-post-externalsponsors.md) | Nenhuma | Adicione um usuário ou grupo a **patrocinadores externos** de uma organização conectada. |
|[Remover internalSponsors](../api/connectedorganization-delete-internalsponsors.md) | Nenhuma | Remova um usuário ou grupo dos **patrocinadores internos de** uma organização conectada. |
|[Remover externalSponsors](../api/connectedorganization-delete-externalsponsors.md) | Nenhuma | Remova um usuário ou grupo dos patrocinadores **externos** de uma organização conectada. |

## <a name="types"></a>Tipos

- [requestorSettings](requestorsettings.md), [approvalSettings](approvalsettings.md), [questions](accesspackagequestion.md) e [assignmentReviewSettings](assignmentreviewsettings.md) - Usado em um [accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) para especificar quem pode solicitar, quem aprova e quem revisa as solicitações de atribuição de pacote de acesso nessa política.
- [approvalStage](approvalstage.md) - Usado nas [approvalSettings](approvalsettings.md) para especificar os aprovadores primários, de backup e de escalonamento.
- [userSet](userset.md) subtypes [singleUser](singleuser.md), [groupMembers](groupmembers.md), [connectedOrganizationMembers](connectedorganizationmembers.md), [requestorManager](requestormanager.md), [internalSponsors](internalsponsors.md)e [externalSponsors](externalsponsors.md) - Usado em [requestorSettings](requestorsettings.md), [approvalStage](approvalstage.md) e [assignmentReviewSettings](assignmentreviewsettings.md).
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
