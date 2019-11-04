---
title: Diferenças de tipo de recurso entre o Azure AD Graph e o Microsoft Graph
description: Descreve as diferenças entre recursos no gráfico do Azure AD e recursos no Microsoft Graph para ajudar a migrar aplicativos.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 925faf5aa27adcdef3d0ade88f9c3d5d8a911c75
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37934736"
---
# <a name="resource-type-differences-between-azure-ad-graph-and-microsoft-graph"></a>Diferenças de tipo de recurso entre o Azure AD Graph e o Microsoft Graph

Este artigo faz parte da *etapa 1: revisar as diferenças de API* do [processo de migração de aplicativos](migrate-azure-ad-graph-planning-checklist.md).

Ao migrar aplicativos do Azure AD Graph para o Microsoft Graph, lembre-se de que alguns recursos têm nomes e tipos diferentes.  Por exemplo, se seu aplicativo do Azure AD Graph usa o recurso **tenantInfo** , você precisará atualizar seu código para se referir à [organização](/graph/api/resources/organization?view=graph-rest-1.0) .

A tabela a seguir realça as diferenças entre o Azure AD Graph e recursos do Microsoft Graph.  Ele mostra recursos com nomes diferentes ou que não estão disponíveis; Ele também realça os recursos disponíveis na versão beta do Microsoft Graph, mas não na versão v 1.0.

Se um recurso não for mostrado na lista, ele já estará disponível na [versão v 1.0](/graph/api/overview?view=graph-rest-1.0) do Microsoft Graph, com o mesmo nome do gráfico do Azure AD.

> **Observação**: os nomes de tipo de recurso no Azure ad Graph são Pascal-case, enquanto no Microsoft Graph eles são camel-case.

|Azure AD Graph. <br>(v 1.6) Resource |Microsoft Graph<br>recurso|Comentários|
|---|---|---|
| [Application](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | Beta- [aplicativo](/graph/api/resources/application?view=graph-rest-beta)<br>v 1.0- [Application](/graph/api/resources/application?view=graph-rest-1.0) ||
| [AppRole](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | Beta- [appRole](/graph/api/resources/approle?view=graph-rest-beta)<br>v 1.0- [appRole](/graph/api/resources/appRole?view=graph-rest-1.0) | |
| [AppRoleAssignment](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | versão&nbsp;-&nbsp;beta[appRoleAssignment](/graph/api/resources/approleassignment?view=graph-rest-beta)<br>v 1.0- _ainda não disponível_ | |
| [CertificateAuthorityInformation](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | versão&nbsp;-&nbsp;beta[certificateAuthority](/graph/api/resources/certificateauthority?view=graph-rest-beta)<br>v 1.0&nbsp;-&nbsp;[certificateAuthority](/graph/api/resources/certificateauthority?view=graph-rest-v1.0) | |
| [Contato](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | Beta- [orgContact](/graph/api/resources/orgContact?view=graph-rest-beta)<br>v 1.0- [orgContact](/graph/api/resources/orgContact?view=graph-rest-v1.0) | |
| [DirectoryLinkChange](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | Beta- _nova&nbsp;abordagem_ <br>v 1.0- _nova&nbsp;abordagem_ | A consulta Delta oferece suporte à detecção de alteração de relação com um mecanismo que não requer esse recurso. Consulte [diferenças de recursos entre o Azure ad Graph e o Microsoft Graph](migrate-azure-ad-graph-feature-differences.md). |
| [OAuth2Permission](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | Beta- [permissionScope](/graph/api/resources/permissionScope?view=graph-rest-beta) <br> v 1.0- [permissionScope](/graph/api/resources/permissionScope?view=graph-rest-1.0) ||
| [OAuth2PermissionGrant](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | versão&nbsp;-&nbsp;beta[oAuth2PermissionGrant](/graph/api/resources/oAuth2PermissionGrant?view=graph-rest-beta) <br> v 1.0- _ainda não disponível_ ||
| [PasswordProfile](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | Beta- [passwordProfile](/graph/api/resources/passwordProfile?view=graph-rest-beta) <br> v 1.0-PasswordProfile ||
| [Política](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | Beta- [política](/graph/api/resources/parentalcontrolsettings?view=graph-rest-beta) _(sujeita a alterações)_ <br> v 1.0- _ainda não disponível_ | Cada política terá um nome de tipo exclusivo e uma estrutura.|
| [ProvisioningError](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | versão&nbsp;-&nbsp;beta_não disponível_ <br> v 1.0&nbsp;-&nbsp;_não disponível_ | Esse recurso foi preterido.  No entanto, um novo recurso descrevendo quaisquer erros de provisionamento relacionados ao AD Connect pode ser encontrado no [onPremisesProvisioningError](/graph/api/resources/onPremisesProvisioningError?view=graph-rest-v1.0). |
| [ServiceEndpoint](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | Beta- [ponto de extremidade](/graph/api/resources/endpoint?view=graph-rest-beta) <br> v 1.0-ponto de extremidade _ainda não disponível_ | o [ponto de extremidade](/graph/api/resources/endpoint?view=graph-rest-beta) só está disponível como parte do recurso de [grupo](/graph/api/resources/group?view=graph-rest-beta) .|
| [ServicePrincipal](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | Beta- [servicePrincipalName](/graph/api/resources/serviceprincipal?view=graph-rest-beta) <br> v 1.0- _ainda não disponível_ | |
| [SignInName](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | Beta- _ainda não disponível_ <br> v 1.0- _ainda não disponível_ | Nova modelagem para os identificadores usados para entrar em uma conta de usuário, chamada **identityobject**, mas ainda não disponível. Oferece suporte a cenários do Azure AD B2C. |
| [TenantDetail](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | Beta- [organização](/graph/api/resources/organization?view=graph-rest-beta) <br> v 1.0- [organização](/graph/api/resources/organization?view=graph-rest-v1.0) | |
| [TrustedCasForPasswordAuth](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | versão&nbsp;-&nbsp;beta[certificateBasedAuthConfiguration](/graph/api/resources/certificatebasedcuthconfiguration?view=graph-rest-beta) <br> v 1.0&nbsp;-&nbsp;[certificateBasedAuthConfiguration](/graph/api/resources/certificatebasedcuthconfiguration?view=graph-rest-v1.0) | |
| [UserIdentity](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | Beta- _ainda não disponível_ <br> v 1.0- _ainda não disponível_ |  Nova modelagem para os identificadores usados para entrar em uma conta de usuário, chamada **identityobject**, mas ainda não disponível. Oferece suporte a cenários do Azure AD B2C. |

## <a name="next-steps"></a>Próximas etapas

- Saiba mais sobre as [diferenças de propriedade de entidade](migrate-azure-ad-graph-property-differences.md) entre o Azure ad Graph e o Microsoft Graph.
- Explore os conceitos e as práticas [do Microsoft Graph](/graph/overview) .
- Use o [Explorador do Graph](https://aka.ms/ge) para experimentar o Microsoft Graph.
