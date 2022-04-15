---
title: Trabalhando com grupos no Microsoft Graph
description: Grupos são coleções de entidades de segurança com acesso compartilhado a recursos em serviços Microsoft ou no seu aplicativo. Diferentes entidades de segurança, como usuários, outros grupos, dispositivos e aplicativos, podem fazer parte de grupos. O uso de grupos ajuda você a evitar trabalhar com entidades de segurança individuais e simplifica o gerenciamento do acesso aos seus recursos.
author: psaffaie
ms.localizationpriority: high
ms.prod: groups
doc_type: conceptualPageType
ms.openlocfilehash: 39855db405aeac9d6f8896e04fdd4fa25067cc0d
ms.sourcegitcommit: b21ad24622e199331b6ab838a949ddce9726b41b
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2022
ms.locfileid: "64848528"
---
# <a name="working-with-groups-in-microsoft-graph"></a>Trabalhando com grupos no Microsoft Graph

Grupos são coleções de entidades de segurança com acesso compartilhado a recursos em serviços Microsoft ou no seu aplicativo. Diferentes entidades de segurança, como usuários, outros grupos, dispositivos e aplicativos, podem fazer parte de grupos. O uso de grupos ajuda você a evitar trabalhar com entidades de segurança individuais e simplifica o gerenciamento do acesso aos seus recursos.

O Microsoft Graph expõe a API de grupos para criar e gerenciar diferentes tipos de grupos e funcionalidades de grupo. 

> [!NOTE]
> 1. Os grupos só podem ser criados por meio de contas corporativas ou de estudante. As contas pessoais da Microsoft não são compatíveis com grupos.
> 2. Todas as operações relacionadas a grupos no Microsoft Graph exigem autorização do administrador.

## <a name="group-types-in-azure-ad-and-microsoft-graph"></a>Tipos de grupo no Azure AD e no Microsoft Graph

O Azure Active Directory (Microsoft Azure AD) suporta os seguintes tipos de grupos.

- Grupos do Microsoft 365
- Grupos de segurança
- Grupos de segurança habilitados para email
- Grupos de distribuição

Somente grupos de segurança e do Microsoft 365 podem ser gerenciados por meio da API de grupos do Microsoft Graph. Grupos de distribuição e habilitados para email são somente leitura por meio do Microsoft Graph.

No Microsoft Graph, o tipo de grupo pode ser identificado pelas configurações de suas propriedades **groupType**, **mailEnabled** e **securityEnabled** conforme indicado na tabela abaixo.

| Tipo |groupType | mailEnabled | securityEnabled | Criado e gerenciado através da API de grupos |
|--|--|--|--|--|
| [Grupos do Microsoft 365](#microsoft-365-groups) | `["Unified"]` | `true` | `true` ou `false` | Sim |
| [Grupos de segurança](#security-groups-and-mail-enabled-security-groups) | `[]` | `false` | `true` | Sim |
| [Grupos de segurança habilitados para email](#security-groups-and-mail-enabled-security-groups) | `[]` | `true` | `true` | Não |
| Grupos de distribuição | `[]` | `true` | `false` | Não |

Para obter mais informações sobre grupos, consulte as seções abaixo. Para obter mais informações sobre grupos no Microsoft Azure AD, consulte [comparar grupos no Microsoft Azure AD](/microsoft-365/admin/create-groups/compare-groups).

## <a name="microsoft-365-groups"></a>Grupos do Microsoft 365

O diferencial dos grupos da Microsoft 365 está na natureza cooperativa, perfeito para as pessoas que trabalham em conjunto em um projeto ou uma equipe. Eles são criados com recursos que os membros do grupo compartilham, incluindo:

- Conversas do Outlook
- Calendário do Outlook
- Arquivos do SharePoint
- Bloco de anotações do OneNote
- Site de equipe do SharePoint
- Planos do Planner
- Gerenciamento de dispositivos do Microsoft Intune

O objeto JSON a seguir mostra um exemplo de representação de um grupo quando você chama a API de grupos do Microsoft Graph.

```http
HTTP/1.1 201 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups/$entity",
    "id": "4c5ee71b-e6a5-4343-9e2c-4244bc7e0938",
    "deletedDateTime": null,
    "classification": "MBI",
    "createdDateTime": "2016-08-23T14:46:56Z",
    "description": "This is a group in Outlook",
    "displayName": "OutlookGroup101",
    "groupTypes": [
        "Unified"
    ],
    "mail": "outlookgroup101@service.microsoft.com",
    "mailEnabled": true,
    "mailNickname": "outlookgroup101",
    "preferredLanguage": null,
    "proxyAddresses": [
        "smtp:outlookgroup101@microsoft.onmicrosoft.com",
        "SMTP:outlookgroup101@service.microsoft.com"
    ],
    "securityEnabled": false,
    "theme": null,
    "visibility": "Public"
}
```

Para saber mais sobre os grupos do Microsoft 365 e as experiências de administrador, confira [Saiba mais sobre grupos do Microsoft 365](https://support.office.com/article/Learn-about-Office-365-groups-b565caa1-5c40-40ef-9915-60fdb2d97fa2).

## <a name="security-groups-and-mail-enabled-security-groups"></a>Grupos de segurança e grupos de segurança habilitados para email.

Os **grupos de segurança** servem para controlar o acesso do usuário aos recursos. Ao verificar se um usuário faz parte de um grupo de segurança, seu aplicativo pode tomar decisões de autorização quando esse usuário tentar acessar alguns recursos seguros do seu aplicativo. Os grupos de segurança podem ter usuários, outros grupos de segurança, dispositivos e entidades de serviço como membros.

Os **grupos de segurança habilitados para email** são usados da mesma forma que os grupos de segurança, mas com o recurso adicional de uma caixa de correio compartilhada. Os grupos de segurança habilitados para email não podem ser criados ou atualizados por meio da API; em vez disso, eles são somente leitura. Saiba mais no artigo [Gerenciar de grupos de segurança habilitados para email no Exchange](/Exchange/recipients/mail-enabled-security-groups).

O objeto JSON a seguir mostra um exemplo de representação de um grupo quando você chama a API de grupos do Microsoft Graph.

```http
HTTP/1.1 201 OK
Content-type: application/json

{
    "@odata.type": "#microsoft.graph.group",
    "id": "f87faa71-57a8-4c14-91f0-517f54645106",
    "deletedDateTime": null,
    "classification": null,
    "createdDateTime": "2016-07-20T09:21:23Z",
    "description": "This group is a Security Group",
    "displayName": "SecurityGroup101",
    "groupTypes": [],
    "mail": null,
    "mailEnabled": false,
    "mailNickname": "",
    "preferredLanguage": null,
    "proxyAddresses": [],
    "securityEnabled": true
}
```

## <a name="dynamic-membership"></a>Associação dinâmica

Todos os tipos de grupos podem ter regras dinâmicas de associação que adicionam ou removem automaticamente membros do grupo com base nas propriedades da entidade de segurança. Por exemplo, um grupo "Funcionários de marketing" pode definir uma regra de associação dinâmica que apenas os usuários com suas propriedades de departamento definidas como "Marketing" podem ser membros do grupo. Nesse caso, todos os usuários que saem do departamento são automaticamente removidos do grupo. 

As regras de associação dinâmica são especificadas através da propriedade **membershipRule** durante a criação do grupo. Por exemplo, `"membershipRule": 'user.department -eq "Marketing"'`. A propriedade **groupType** também deve incluir o valor `"DynamicMembership"` na coleção. A regra de associação dinâmica pode ser ativada ou desativada através da propriedade **membershipRuleProcessingState**.

O exemplo de solicitação de a seguir cria um novo grupo do Microsoft 365 que só pode incluir funcionários no departamento de Marketing.

```http
POST https://graph.microsoft.com/beta/groups
Content-type: application/json

{
    "description": "Marketing department folks",
    "displayName": "Marketing department",
    "groupTypes": [
        "Unified",
        "DynamicMembership"
    ],
    "mailEnabled": true,
    "mailNickname": "marketing",
    "securityEnabled": false,
    "membershipRule": "'user.department -eq 'Marketing'",
    "membershipRuleProcessingState": "on"
}
```

Para saber mais sobre a formulação de regras de associação, consulte [Regras de associação dinâmicas para grupos no Microsoft Azure AD](/azure/active-directory/enterprise-users/groups-dynamic-membership).

> **Observação**: as regras de associação dinâmica exigem que o locatário tenha pelo menos uma licença do Azure AD Premium P1 para cada usuário exclusivo que seja membro de um ou mais grupos dinâmicos.

## <a name="other-types-of-groups"></a>Outros tipos de grupos

Os grupos do Microsoft 365 no Yammer são usados para facilitar a colaboração de usuários por meio de postagens no Yammer. Esse tipo de grupo pode ser retornado por meio de uma solicitação de leitura, mas as postagens nele não podem ser acessadas por meio da API. Quando as postagens e os feeds de conversas do Yammer são habilitados em um grupo, as conversas padrão em grupo do Microsoft 365 são desabilitadas. Saiba mais em [Documentos de API do desenvolvedor do Yammer](https://developer.yammer.com/docs).

## <a name="group-based-licensing"></a>Licenciamento com base em grupo

O recurso de licenciamento baseado em grupo pode ser usado para atribuir uma ou mais licenças de produto a um grupo do Azure AD. O Azure AD garante que as licenças sejam atribuídas a todos os membros do grupo. Todos os novos membros que ingressarem no grupo receberão as licenças apropriadas. Quando eles deixarem o grupo, essas licenças serão removidas. O recurso pode ser usado apenas com grupos de segurança e grupos do Microsoft 365 que tenham a propriedade **securityEnabled** definida como `true`. Para saber mais sobre o licenciamento com base em grupo, confira [O que é licenciamento com base em grupo no Azure Active Directory?](/azure/active-directory/fundamentals/active-directory-licensing-whatis-azure-portal?context=/azure/active-directory/enterprise-users/context/ugr-context)

## <a name="common-use-cases-for-the-groups-api-in-microsoft-graph"></a>Casos de uso comum para a API de grupos no Microsoft Graph

Usando o Microsoft Graph, você pode executar as seguintes operações comuns nos grupos.

| **Casos de uso** | **Recursos REST** | **Confira também** |
|:-|:-|:-|
| **Criar grupos, gerenciar as características do grupo** |  |  |
| Criar novos grupos, obter os grupos existentes, atualizar as propriedades nos grupos e excluir grupos. Atualmente, somente os grupos de segurança e grupos no Outlook podem ser criados por meio da API. | [grupo](group.md) | [Criar novos grupos](../api/group-post-groups.md) <br/> [Listar grupos](../api/group-list.md) <br/> [Atualizar grupos](../api/group-update.md) <br/> [Excluir grupos](../api/group-delete.md) |
| **Gerenciar a associação a um grupo** |  |  |
| Listar os membros de um grupo e adicionar ou remover membros. | [usuário](user.md) <br/> [grupo](group.md) | [Listar membros](../api/group-list-members.md) <br/> [Adicionar membro](../api/group-post-members.md) <br/> [Remover membro](../api/group-delete-members.md) |
| Determinar se um usuário faz parte de um grupo, acessar todos os grupos do qual o usuário faz parte. | [usuário](user.md) <br/> [group](group.md) <br/> [servicePrincipal](serviceprincipal.md) <br/> [orgContact](orgcontact.md) | [Verificar grupos de membros](../api/directoryobject-checkmembergroups.md) <br/> [Obter grupos de membros](../api/directoryobject-getmembergroups.md) |
| Listar os proprietários de um grupo e adicionar ou remover proprietários. | [usuário](user.md) <br/> [grupo](group.md) | [Listar proprietários](../api/group-list-members.md) <br/> [Adicionar membro](../api/group-post-members.md) <br/> [Remover membro](../api/group-delete-members.md) |

## <a name="whats-new"></a>Novidades

Saiba mais sobre os [recursos e atualizações mais recentes](/graph/whats-new-overview) para a API de grupos.