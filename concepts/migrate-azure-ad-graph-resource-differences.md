---
title: Diferenças de tipo de recurso entre o Azure AD Graph e o Microsoft Graph
description: Descreve as diferenças entre recursos no gráfico do Azure AD e recursos no Microsoft Graph para ajudar a migrar aplicativos.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 590ec2fae33e5172e274341793c82409a4c28c8c
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33630199"
---
# <a name="resource-type-differences-between-azure-ad-graph-and-microsoft-graph"></a>Diferenças de tipo de recurso entre o Azure AD Graph e o Microsoft Graph

Este artigo faz parte da *etapa 1:* revisar as diferenças de API do [processo de migração de aplicativos](migrate-azure-ad-graph-planning-checklist.md).

Ao migrar aplicativos do Azure AD Graph para o Microsoft Graph, lembre-se de que alguns recursos têm nomes e tipos diferentes.  Por exemplo, se seu aplicativo do Azure AD Graph usa o recurso **tenantInfo** , você precisará atualizar seu código para se referir à [organização](/graph/api/resources/organization?view=graph-rest-1.0) .

A tabela a seguir realça as diferenças entre o Azure AD Graph e recursos do Microsoft Graph.  Ele mostra recursos com nomes diferentes ou que não estão disponíveis; Ele também realça os recursos disponíveis na versão beta do Microsoft Graph, mas não na versão v 1.0.

Se um recurso não for mostrado na lista, ele já estará disponível na [versão v 1.0](/graph/api/overview?view=graph-rest-1.0) do Microsoft Graph, com o mesmo nome do gráfico do Azure AD.

> **Observação**: os nomes de tipo de recurso no Azure ad Graph são Pascal-case, enquanto no Microsoft Graph eles são camel-case.

|Gráfico do Azure AD <br>(v 1.6) Resource |Microsoft Graph<br>recurso|Comments|
|---|---|---|
| [Caligrafia](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference)       | Beta- _ainda não disponível_<br>v 1.0- _ainda não disponível_ ||
| [Aplicativo](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | Beta- [aplicativo](/graph/api/resources/application?view=graph-rest-beta)<br>v 1.0- _ainda não disponível_ ||
| [AppRole](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | Beta- [appRole](/graph/api/resources/approle?view=graph-rest-beta)<br>v 1.0- _ainda não disponível_ | |
| [AppRoleAssignment](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | versão&nbsp;-&nbsp;beta[appRoleAssignment](/graph/api/resources/approleassignment?view=graph-rest-beta)<br>v 1.0- _ainda não disponível_ | |
| [Contact](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | Beta- [orgContact](/graph/api/resources/orgContact?view=graph-rest-beta)<br>v 1.0- _ainda não disponível_ | |
| [DirectoryLinkChange](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | Beta- _nova&nbsp;abordagem_ <br>v 1.0- _nova&nbsp;abordagem_ | A consulta Delta oferece suporte à detecção de alteração de relação com um mecanismo que não requer esse recurso. Consulte [diferenças de recursos entre o Azure ad Graph e o Microsoft Graph](migrate-azure-ad-graph-feature-differences.md). |
| [Keycredential](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference)| Beta- [Keycredential](/graph/api/resources/keyCredential?view=graph-rest-beta)<br>v 1.0- _ainda não disponível_ | |
| [Chavevalor](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | Beta- [KeyValue](/graph/api/resources/keyValue?view=graph-rest-beta) <br> v 1.0- _ainda não disponível_ ||
| [OAuth2Permission](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | Beta- [permissionScope](/graph/api/resources/permissionScope?view=graph-rest-beta) <br> v 1.0- _ainda não disponível_ ||
| [OAuth2PermissionGrant](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | versão&nbsp;-&nbsp;beta[oAuth2PermissionGrant](/graph/api/resources/oAuth2PermissionGrant?view=graph-rest-beta) <br> v 1.0- _ainda não disponível_ ||
| [OptionalClaim](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | Beta-optionalClaim <br> v 1.0- _ainda não disponível_ | |
| [OptionalClaims](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | Beta-optionalClaims<br> v 1.0- _ainda não disponível_ ||
| [ParentalControlSettings](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | Beta- [parentalControlSettings](/graph/api/resources/parentalcontrolsettings?view=graph-rest-beta) <br> v 1.0- _ainda não disponível_ ||
| [PasswordCredential](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | Beta- [passwordCredential](/graph/api/resources/passwordCredential?view=graph-rest-beta) <br> v 1.0- _ainda não disponível_ ||
| [PasswordProfile](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | Beta- [passwordProfile](/graph/api/resources/passwordProfile?view=graph-rest-beta) <br> v 1.0-PasswordProfile ||
| [Política](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | Beta- [política](/graph/api/resources/parentalcontrolsettings?view=graph-rest-beta) _(sujeita a alterações)_ <br> v 1.0- _ainda não disponível_ | Cada política terá um nome de tipo exclusivo e uma estrutura.|
| [ProvisioningError](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | versão&nbsp;-&nbsp;beta[onPremisesProvisioningError](/graph/api/resources/onPremisesProvisioningError?view=graph-rest-beta) <br> v 1.0&nbsp;-&nbsp;onPremisesProvisioningError  | |
| [RequiredResourceAccess](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | Beta- [requiredResourceAccess](/graph/api/resources/requiredResourceAccess?view=graph-rest-beta) <br> v 1.0- _ainda não disponível_ | |
| [ResourceAccess](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | Beta- [resourceAccess](/graph/api/resources/resourceAccess?view=graph-rest-beta) <br> v 1.0- _ainda não disponível_ | |
| [ServiceEndpoint](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | Beta- [ponto de extremidade](/graph/api/resources/endpoint?view=graph-rest-beta) <br> v 1.0-ponto de extremidade _ainda não disponível_ | o [ponto de extremidade](/graph/api/resources/endpoint?view=graph-rest-beta) só está disponível como parte do recurso de [grupo](/graph/api/resources/group?view=graph-rest-beta)|
| [ServicePrincipal](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | Beta- [servicePrincipalName](/graph/api/resources/serviceprincipal?view=graph-rest-beta) <br> v 1.0- _ainda não disponível_ | |
| [SignInName](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | Beta- _ainda não disponível_ <br> v 1.0- _ainda não disponível_ | Nova modelagem para os identificadores usados para entrar em uma conta de usuário, **** chamada identityobject, mas ainda não disponível. Oferece suporte a cenários do Azure AD B2C. |
| [TenantDetail](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | Beta- [organização](/graph/api/resources/organization?view=graph-rest-beta) <br> v 1.0- [organização](/graph/api/resources/organization?view=graph-rest-v1.0) | |
| [TrustedCasForPasswordAuth](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | versão&nbsp;-&nbsp;beta_ainda não disponível_ <br> v 1.0- _ainda não disponível_  | Renomeando para **certificateBasedAuthConfiguration** , mas ainda não disponível.|
| [UserIdentity](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | Beta- _ainda não disponível_ <br> v 1.0- _ainda não disponível_ |  Nova modelagem para os identificadores usados para entrar em uma conta de usuário, **** chamada identityobject, mas ainda não disponível. Oferece suporte a cenários do Azure AD B2C. |

## <a name="next-steps"></a>Próximos passos

- Saiba mais sobre as [diferenças de propriedade de entidade](migrate-azure-ad-graph-property-differences.md) entre o Azure ad Graph e o Microsoft Graph.
- Explore os conceitos e as práticas [do Microsoft Graph](/graph/overview) .
- Use o [Explorador do Graph](https://aka.ms/ge) para experimentar o Microsoft Graph.
