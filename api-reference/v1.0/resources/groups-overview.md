---
title: Trabalhando com grupos no Microsoft Graph
description: Os grupos são conjuntos de usuários e de outras entidades de segurança que compartilham o acesso a recursos nos serviços Microsoft ou em seu aplicativo. O Microsoft Graph fornece APIs que você pode usar para criar e gerenciar os diferentes tipos e funcionalidades de grupo de acordo com seu cenário. Todas as operações relacionadas a grupos no Microsoft Graph exigem autorização do administrador.
author: Jordanndahl
ms.localizationpriority: high
ms.prod: groups
doc_type: conceptualPageType
ms.openlocfilehash: bb455ffde8ab93ed0c93fcb35cdb088f2ce6979f
ms.sourcegitcommit: 9adf70c5da7c5b65f7d20f571d101ee06f023bc3
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/25/2022
ms.locfileid: "62201691"
---
# <a name="working-with-groups-in-microsoft-graph"></a>Trabalhando com grupos no Microsoft Graph

Os grupos são coleções de [usuários](user.md) e de outras entidades de segurança que compartilham o acesso a recursos nos serviços Microsoft ou em seu aplicativo. O Microsoft Graph fornece APIs que você pode usar para criar e gerenciar os diferentes tipos e funcionalidades de grupo de acordo com seu cenário. Todas as operações relacionadas a grupos no Microsoft Graph exigem autorização do administrador.

> **Observação**: os grupos só podem ser criados por meio de contas corporativas ou de estudante. As contas pessoais da Microsoft não são compatíveis com grupos.

## <a name="group-types-in-azure-ad-and-microsoft-graph"></a>Tipos de grupo no Azure AD e no Microsoft Graph

O Azure AD suporta os seguintes tipos de grupos.

+ Grupos do Microsoft 365
+ Grupos de segurança
+ Grupos de segurança habilitados para email
+ Grupos de distribuição

Para obter mais informações sobre grupos do Azure AD, confira [comparar grupos no Azure AD](/microsoft-365/admin/create-groups/compare-groups).

No Microsoft Graph, o tipo de grupo pode ser identificado pelas configurações de suas propriedades **groupType**, **mailEnabled** e **securityEnabled** conforme indicado na tabela abaixo.

| Tipo              | Caso de uso | groupType | mailEnabled | securityEnabled | Criado e gerenciado via API |
|-------------------|----------|-----------|--------------|------------------|--------------------------------|
| [Grupos do Microsoft 365](#microsoft-365-groups) | Facilitar a colaboração entre usuários com os recursos compartilhados online da Microsoft. | `["Unified"]` | `true` | `true` ou `false` | Sim |
| [Grupos de segurança](#security-groups-and-mail-enabled-security-groups) | Controlar o acesso do usuário aos recursos do aplicativo. | `[]` | `false` | `true` | Sim |
| [Grupos de segurança habilitados para email](#security-groups-and-mail-enabled-security-groups) | Controlar o acesso do usuário aos recursos do aplicativo, com uma caixa de correio de grupo compartilhada. | `[]` | `true` | `true` | Não |
| Grupos de distribuição | Distribuir emails aos membros do grupo. É recomendável usar os grupos do Microsoft 365 devido a grande quantidade de recursos que ele fornece. | `[]` | `true` | `false` | Não |


## <a name="microsoft-365-groups"></a>Grupos do Microsoft 365
O diferencial dos grupos da Microsoft 365 está na natureza cooperativa, perfeito para as pessoas que trabalham em conjunto em um projeto ou uma equipe. Eles são criados com recursos compartilhados pelos membros do grupo, entre eles:

- Conversas do Outlook
- Calendário do Outlook
- Arquivos do SharePoint
- Bloco de anotações do OneNote
- Site de equipe do SharePoint
- Planos do Planner
- Gerenciamento de dispositivos do Microsoft Intune

### <a name="group-in-outlook-example"></a>Grupo em um exemplo do Outlook

Veja a seguir uma representação JSON dos grupos no Outlook.

```http

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

Os grupos de segurança servem para controlar o acesso de usuários aos recursos. Ao verificar se um usuário faz parte de um grupo de segurança, seu aplicativo pode tomar decisões de autorização quando esse usuário tentar acessar alguns recursos seguros do seu aplicativo. Os grupos de segurança podem ter como membros usuários e outros grupos de segurança.

Os grupos de segurança habilitados para email são usados da mesma forma que os grupos de segurança, mas com o recurso adicional de uma caixa de correio compartilhada para os grupos. Grupos de segurança habilitados para email são somente leitura. Saiba mais no artigo [Gerenciar de grupos de segurança habilitados para email no Exchange](/Exchange/recipients/mail-enabled-security-groups).

### <a name="security-group-example"></a>Exemplo de grupo de segurança

Veja a seguir uma representação JSON de um grupo de segurança.

```http
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

Todos os tipos de grupo podem ter regras de associação dinâmica que adicionam ou removem automaticamente membros do grupo com base nas propriedades do usuário. Por exemplo, um grupo de "funcionários do Marketing" pode incluir todo usuário que tiver a propriedade departament definida como "Marketing". Dessa forma, os novos funcionários de marketing são adicionados automaticamente ao grupo, enquanto os que saem do departamento são automaticamente removidos dele. Essa regra pode ser especificada em um campo "membershipRule" durante a criação de grupo como `"membershipRule": 'user.department -eq "Marketing"'`. O GroupType também deve incluir a `"DynamicMembership"`. A solicitação a seguir cria um novo grupo do Microsoft 365 para os funcionários de marketing:

```http
POST https://graph.microsoft.com/beta/groups
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
    "membershipRule": "user.department -eq \"Marketing\"",
    "membershipRuleProcessingState": "on"
}
```

Saiba como formular membershipRules no artigo [Criar regras baseadas em atributo para associação dinâmica de grupo no Azure Active Directory](/azure/active-directory/active-directory-groups-dynamic-membership-azure-portal).

> **Observação**: as regras de associação dinâmica exigem que o locatário tenha uma licença ao nível [Azure Active Directory Premium P1](https://azure.microsoft.com/pricing/details/active-directory/) ou posterior.

## <a name="other-types-of-groups"></a>Outros tipos de grupos

Os grupos do Microsoft 365 no Yammer são usados para facilitar a colaboração de usuários por meio de postagens no Yammer. Esse tipo de grupo pode ser retornado por meio de uma solicitação de leitura, mas as postagens nele não podem ser acessadas por meio da API. Quando as postagens e os feeds de conversas do Yammer são habilitados em um grupo, as conversas padrão em grupo do Microsoft 365 são desabilitadas. Saiba mais em [Documentos de API do desenvolvedor do Yammer](https://developer.yammer.com/docs).

## <a name="group-based-licensing"></a>Licenciamento com base em grupo

Você pode usar o licenciamento com base em grupo para atribuir uma ou mais licenças de produto a um grupo do Azure AD. O Azure AD garante que as licenças sejam atribuídas a todos os membros do grupo. Todos os novos membros que ingressarem no grupo receberão as licenças apropriadas. Quando eles deixarem o grupo, essas licenças serão removidas. O recurso só pode ser usado com os grupos de segurança e grupos do Microsoft 365 que possuam `securityEnabled=TRUE`. Para saber mais sobre o licenciamento com base em grupo, confira [O que é licenciamento com base em grupo no Azure Active Directory?](/azure/active-directory/fundamentals/active-directory-licensing-whatis-azure-portal)

## <a name="common-use-cases"></a>Casos de usos comuns

Ao usar o Microsoft Graph, você pode executar as seguintes operações comuns.

| **Casos de uso**  | **Recursos REST** | **Confira também** |
|:---------------|:--------|:----------|
| **Métodos e objetos de grupo** | | |
| Criar novos grupos, obter os grupos existentes, atualizar as propriedades nos grupos e excluir grupos. Atualmente, somente os grupos de segurança e grupos no Outlook podem ser criados por meio da API. | [grupo](group.md) | [Criar novos grupos](../api/group-post-groups.md) <br/> [Listar grupos](../api/group-list.md) <br/> [Atualizar grupos](../api/group-update.md) <br/> [Excluir grupos](../api/group-delete.md) |
| **Métodos de associação a grupos** | | |
| Listar os membros de um grupo e adicionar ou remover membros. | [usuário](user.md) <br/> [grupo](group.md)| [Listar membros](../api/group-list-members.md) <br/> [Adicionar membro](../api/group-post-members.md) <br/> [Remover membro](../api/group-delete-members.md)|
| Determinar se um usuário faz parte de um grupo, acessar todos os grupos do qual o usuário faz parte. | [usuário](user.md) <br/> [group](group.md) <br/> [servicePrincipal](serviceprincipal.md) <br/> [orgContact](orgcontact.md)| [Verificar grupos de membros](../api/directoryobject-checkmembergroups.md) <br/> [Obter grupos de membros](../api/directoryobject-getmembergroups.md)|
| Listar os proprietários de um grupo e adicionar ou remover proprietários. | [usuário](user.md) <br/> [grupo](group.md)| [Listar proprietários](../api/group-list-members.md) <br/> [Adicionar membro](../api/group-post-members.md) <br/> [Remover membro](../api/group-delete-members.md)|

## <a name="whats-new"></a>Novidades
Saiba mais sobre os [novos recursos e atualizações mais recentes](/graph/whats-new-overview) para este conjunto de APIs.
