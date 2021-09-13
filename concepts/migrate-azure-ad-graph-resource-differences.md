---
title: Diferenças de tipo de recurso entre o Azure Active Directory (Azure AD) Graph e o Microsoft Graph
description: Descreve as diferenças entre recursos no Azure Active Directory (Azure AD) Graph e recursos no Microsoft Graph para ajudar a migrar aplicativos.
author: dkershaw10
ms.localizationpriority: medium
ms.prod: applications
ms.openlocfilehash: ffd0f23c417ead7fa8457bac9ef8cd00e10f1dcd
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59044248"
---
# <a name="resource-type-differences-between-azure-active-directory-azure-ad-graph-and-microsoft-graph"></a>Diferenças de tipo de recurso entre o Azure Active Directory (Azure AD) Graph e o Microsoft Graph

Este artigo faz parte da *etapa 1: analisar as* diferenças de API do processo para [migrar aplicativos.](migrate-azure-ad-graph-planning-checklist.md)

Ao migrar aplicativos do Azure AD Graph para o Microsoft Graph, esteja ciente de que alguns recursos têm nomes diferentes e tipos diferentes.  Por exemplo, se seu aplicativo do Azure AD Graph usar o recurso **tenantInfo,** você precisará atualizar seu código para se referir à [organização.](/graph/api/resources/organization)

A tabela a seguir destaca as diferenças entre os recursos do Azure AD Graph microsoft Graph recursos.  Ele mostra recursos que têm nomes diferentes ou não estão disponíveis; ele também realça os recursos disponíveis na versão beta do Microsoft Graph, mas não na versão v1.0.

Se um  recurso não for mostrado nesta lista, ele já estará disponível na [versão v1.0](/graph/api/overview) do Microsoft Graph, com o mesmo nome do Azure AD Graph.

> **OBSERVAÇÃO**: os nomes de tipo de recurso no Azure AD Graph são em caso pascal, enquanto na Microsoft Graph eles são camel-cased.

|Azure AD Graph. <br>Recurso (v1.6) |Microsoft Graph<br>recurso|Comentários|
|---|---|---|
| [CertificateAuthorityInformation](/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | beta &nbsp; - &nbsp; [certificateAuthority](/graph/api/resources/certificateauthority?view=graph-rest-beta&preserve-view=true)<br>v1.0 &nbsp; - &nbsp; [certificateAuthority](/graph/api/resources/certificateauthority) | |
| [Contato](/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | beta &nbsp; - &nbsp; [orgContact](/graph/api/resources/orgContact?view=graph-rest-beta&preserve-view=true)<br>v1.0 &nbsp; - &nbsp; [orgContact](/graph/api/resources/orgContact) | |
| [DirectoryLinkChange](/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | beta &nbsp; - &nbsp; _Nova &nbsp; abordagem_ <br>v1.0 &nbsp; - &nbsp; _Nova &nbsp; abordagem_ | A consulta delta dá suporte à detecção de alteração de relação com um mecanismo que não exige esse recurso. Confira [Diferenças de recursos entre o Azure AD Graph e o Microsoft Graph](migrate-azure-ad-graph-feature-differences.md). |
| [OAuth2Permission](/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | beta &nbsp; - &nbsp; [permissionScope](/graph/api/resources/permissionScope?view=graph-rest-beta&preserve-view=true) <br> v1.0 &nbsp; - &nbsp; [permissionScope](/graph/api/resources/permissionScope) ||
 [Política](/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | políticas &nbsp; - beta &nbsp; [](/graph/api/resources/policy-overview?view=graph-rest-beta&preserve-view=true) <br> políticas v1.0 &nbsp; - &nbsp; [](/graph/api/resources/policy-overview)| Cada tipo de política tem um nome de tipo exclusivo e uma estrutura, no segmento **de** caminho da URL de políticas, no Microsoft Graph. No Azure AD Graph era um tipo de política único. Por exemplo, para o Azure AD Graph você trabalharia com o recurso **Política** e definiria a propriedade **type** como , enquanto no Microsoft Graph esse seria o recurso `TokenIssuancePolicy` **tokenIssuancePolicy.** |
| [ProvisioningError](/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | beta &nbsp; - &nbsp; _Não disponível_ <br> v1.0 &nbsp; - &nbsp; _Não disponível_ | Esse recurso foi preterido.  No entanto, um novo recurso que descreve qualquer erro de provisionamento Conexão AD pode ser encontrado em [onPremisesProvisioningError](/graph/api/resources/onPremisesProvisioningError). |
| [ServiceEndpoint](/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | ponto &nbsp; - &nbsp; [de extremidade](/graph/api/resources/endpoint?view=graph-rest-beta&preserve-view=true) beta <br> ponto de extremidade v1.0 &nbsp; - &nbsp; [](/graph/api/resources/endpoint) | **os pontos de extremidade** estão disponíveis apenas como parte do recurso [de](/graph/api/resources/group?view=graph-rest-beta&preserve-view=true) grupo na versão beta e o [recurso servicePrincipal](/graph/api/resources/serviceprincipal) em beta e v1.0.|
| [SignInName](/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | beta &nbsp; - &nbsp; _Nova abordagem_ <br> v1.0 &nbsp; - &nbsp; _Nova abordagem_ | Nova modelagem para os identificadores usados para entrar em uma conta de usuário. Consulte [objectIdentity](/graph/api/resources/objectIdentity) resource type para obter mais detalhes. Oferece suporte a cenários do Azure AD B2C. |
| [TenantDetail](/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | organização &nbsp; - beta &nbsp; [](/graph/api/resources/organization?view=graph-rest-beta&preserve-view=true) <br> organização v1.0 &nbsp; - &nbsp; [](/graph/api/resources/organization) | |
| [TrustedCasForPasswordAuth](/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | beta &nbsp; - &nbsp; [certificateBasedAuthConfiguration](/graph/api/resources/certificatebasedcuthconfiguration?view=graph-rest-beta&preserve-view=true) <br> v1.0 &nbsp; - &nbsp; [certificateBasedAuthConfiguration](/graph/api/resources/certificatebasedcuthconfiguration) | |
| [UserIdentity](/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | beta &nbsp; - &nbsp; [objectIdentity](/graph/api/resources/objectidentity?view=graph-rest-beta&preserve-view=true) <br> &nbsp; - &nbsp; [objectIdentity](/graph/api/resources/objectidentity) v1.0 |  Nova modelagem para os identificadores usados para entrar em uma conta de usuário, chamada **objectIdentity**. Oferece suporte a cenários do Azure AD B2C. |

## <a name="next-steps"></a>Próximas etapas

- Saiba mais [sobre as diferenças de](migrate-azure-ad-graph-property-differences.md) propriedades de entidade entre o Azure AD Graph e o Microsoft Graph.
- Revise a [lista de verificação](migrate-azure-ad-graph-planning-checklist.md) novamente.
