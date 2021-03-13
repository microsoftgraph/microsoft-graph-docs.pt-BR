---
title: Diferenças de tipo de recurso entre o Azure AD Graph e o Microsoft Graph
description: Descreve diferenças entre recursos no Azure AD Graph e recursos no Microsoft Graph para ajudar a migrar aplicativos.
author: dkershaw10
localization_priority: Normal
ms.prod: applications
ms.openlocfilehash: 78cfd1a5f817de6c7efbf7dfc3ec05a13ffaa6ea
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50760641"
---
# <a name="resource-type-differences-between-azure-ad-graph-and-microsoft-graph"></a>Diferenças de tipo de recurso entre o Azure AD Graph e o Microsoft Graph

Este artigo faz parte da *etapa 1: analisar as* diferenças de API do processo para [migrar aplicativos.](migrate-azure-ad-graph-planning-checklist.md)

Ao migrar aplicativos do Azure AD Graph para o Microsoft Graph, esteja ciente de que alguns recursos têm nomes diferentes e tipos diferentes.  Por exemplo, se seu aplicativo do Azure AD Graph usar o recurso **tenantInfo,** você precisará atualizar seu código para se referir à [organização.](/graph/api/resources/organization?view=graph-rest-1.0)

A tabela a seguir destaca as diferenças entre os recursos do Azure AD Graph e do Microsoft Graph.  Ele mostra recursos que têm nomes diferentes ou não estão disponíveis; ele também realça os recursos disponíveis na versão beta do Microsoft Graph, mas não na versão v1.0.

Se um recurso não **for** mostrado nesta lista, ele já estará disponível na [versão v1.0](/graph/api/overview?view=graph-rest-1.0) do Microsoft Graph, com o mesmo nome do Azure AD Graph.

> **OBSERVAÇÃO**: Os nomes de tipo de recurso no Azure AD Graph são em caso pascal, enquanto no Microsoft Graph eles são casos de camel.

|Azure AD Graph. <br>Recurso (v1.6) |Microsoft Graph<br>recurso|Comments|
|---|---|---|
| [CertificateAuthorityInformation](/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | beta &nbsp; - &nbsp; [certificateAuthority](/graph/api/resources/certificateauthority?view=graph-rest-beta)<br>v1.0 &nbsp; - &nbsp; [certificateAuthority](/graph/api/resources/certificateauthority?view=graph-rest-1.0) | |
| [Contato](/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | beta &nbsp; - &nbsp; [orgContact](/graph/api/resources/orgContact?view=graph-rest-beta)<br>v1.0 &nbsp; - &nbsp; [orgContact](/graph/api/resources/orgContact?view=graph-rest-1.0) | |
| [DirectoryLinkChange](/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | beta &nbsp; - &nbsp; _Nova &nbsp; abordagem_ <br>v1.0 &nbsp; - &nbsp; _Nova &nbsp; abordagem_ | A consulta delta dá suporte à detecção de alteração de relação com um mecanismo que não exige esse recurso. Confira [Diferenças de recursos entre o Azure AD Graph e o Microsoft Graph.](migrate-azure-ad-graph-feature-differences.md) |
| [OAuth2Permission](/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | beta &nbsp; - &nbsp; [permissionScope](/graph/api/resources/permissionScope?view=graph-rest-beta) <br> v1.0 &nbsp; - &nbsp; [permissionScope](/graph/api/resources/permissionScope?view=graph-rest-1.0) ||
 [Política](/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | políticas &nbsp; - beta &nbsp; [](/graph/api/resources/policy-overview?view=graph-rest-beta) <br> políticas v1.0 &nbsp; - &nbsp; [](/graph/api/resources/policy-overview?view=graph-rest-1.0)| Cada tipo de política tem um nome de tipo exclusivo e uma estrutura, no segmento **de** caminho da URL de políticas, no Microsoft Graph. No Azure AD Graph, esse era um tipo de política único. Por exemplo, para o Azure AD  Graph, você trabalharia com o recurso Política e definiria a propriedade **type** como , enquanto no Microsoft Graph esse seria o recurso `TokenIssuancePolicy` **tokenIssuancePolicy.** |
| [ProvisioningError](/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | beta &nbsp; - &nbsp; _Não disponível_ <br> v1.0 &nbsp; - &nbsp; _Não disponível_ | Esse recurso foi preterido.  No entanto, um novo recurso que descreve qualquer erro de provisionamento relacionado ao AD Connect pode ser encontrado em [onPremisesProvisioningError](/graph/api/resources/onPremisesProvisioningError?view=graph-rest-1.0). |
| [ServiceEndpoint](/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | ponto &nbsp; - &nbsp; [de extremidade](/graph/api/resources/endpoint?view=graph-rest-beta) beta <br> ponto de extremidade v1.0 &nbsp; - &nbsp; [](/graph/api/resources/endpoint?view=graph-rest-1.0) | **os pontos de extremidade** estão disponíveis apenas como parte do recurso [de](/graph/api/resources/group?view=graph-rest-beta) grupo na versão beta e o [recurso servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-1.0) em beta e v1.0.|
| [SignInName](/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | beta &nbsp; - &nbsp; _Nova abordagem_ <br> v1.0 &nbsp; - &nbsp; _Nova abordagem_ | Nova modelagem para os identificadores usados para entrar em uma conta de usuário. Consulte [objectIdentity](/graph/api/resources/objectIdentity?view=graph-rest-1.0) resource type para obter mais detalhes. Oferece suporte a cenários do Azure AD B2C. |
| [TenantDetail](/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | organização &nbsp; - beta &nbsp; [](/graph/api/resources/organization?view=graph-rest-beta) <br> organização v1.0 &nbsp; - &nbsp; [](/graph/api/resources/organization?view=graph-rest-1.0) | |
| [TrustedCasForPasswordAuth](/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | beta &nbsp; - &nbsp; [certificateBasedAuthConfiguration](/graph/api/resources/certificatebasedcuthconfiguration?view=graph-rest-beta) <br> v1.0 &nbsp; - &nbsp; [certificateBasedAuthConfiguration](/graph/api/resources/certificatebasedcuthconfiguration?view=graph-rest-1.0) | |
| [UserIdentity](/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | beta &nbsp; - &nbsp; [objectIdentity](/graph/api/resources/objectidentity?view=graph-rest-beta) <br> &nbsp; - &nbsp; [objectIdentity](/graph/api/resources/objectidentity?view=graph-rest-1.0) v1.0 |  Nova modelagem para os identificadores usados para entrar em uma conta de usuário, chamada **objectIdentity**. Oferece suporte a cenários do Azure AD B2C. |

## <a name="next-steps"></a>Próximas etapas

- Saiba mais [sobre as diferenças de propriedades de entidade](migrate-azure-ad-graph-property-differences.md) entre o Azure AD Graph e o Microsoft Graph.
- Revise a [lista de verificação](migrate-azure-ad-graph-planning-checklist.md) novamente.