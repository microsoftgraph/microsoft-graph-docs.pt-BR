---
title: Visão geral da API de configurações de acesso entre locatários
description: As configurações de acesso entre locatários permitem que você gerencie a colaboração B2B e a conexão direta B2B para sua organização.
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 270f1b53428853c5ba539a94014bec532e10fced
ms.sourcegitcommit: a30eea2fa59087088f50e58706b91c0eb5b7a802
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2022
ms.locfileid: "66604546"
---
# <a name="cross-tenant-access-settings-api-overview"></a>Visão geral da API de configurações de acesso entre locatários

Namespace: microsoft.graph

No modo de Azure AD colaboração B2B, qualquer usuário convidado de uma organização pode usar sua identidade para acessar recursos em organizações externas. Os administradores não têm controle sobre as identidades de usuário em seu locatário que têm permissão para entrar em organizações externas. Esses controles limitados dificultaram o uso de identidades de sua organização de maneiras não autorizadas.

**As configurações de acesso entre locatários** permitem controlar e gerenciar a colaboração entre usuários em sua organização e outras organizações. O controle pode estar no acesso de **saída (como** os usuários colaboram com outras organizações **), no** acesso de entrada (como outras organizações colaboram com você) ou em ambas.

Controles granulares permitem que você determine os usuários, grupos e aplicativos, em sua organização e em organizações externas Azure AD, que podem participar de uma colaboração B2B e Azure AD conexão direta B2B. Esses controles são implementados por meio de:

+ **Configurações de acesso entre locatários** padrão que definem as configurações de acesso de entrada e saída da linha de base.
    + No Azure AD colaboração B2B, as duas configurações de acesso são habilitadas por padrão. Isso significa que todos os usuários podem ser convidados para organizações externas e todos os usuários podem convidar usuários externos.
    + No Azure AD conexão direta B2B, as duas configurações de acesso são desabilitadas por padrão.
    + As configurações padrão do serviço podem ser atualizadas.
+ **Configurações de acesso específicas do parceiro** que permitem definir configurações personalizadas para organizações individuais. Para as organizações configuradas, essa configuração tem precedência sobre as configurações padrão. Portanto, embora Azure AD colaboração B2B e Azure AD conexão direta B2B possam ser desabilitadas em sua organização por padrão, você pode habilitar esses recursos para uma organização externa específica.

> [!IMPORTANT]
> 
> Ao definir as configurações de saída de conexão direta B2B, você concorda em permitir que organizações externas com as quais você habilitou as configurações de saída acessem dados de contato limitados sobre seus usuários. A Microsoft compartilha esses dados com essas organizações para ajudá-las a enviar uma solicitação para se conectar aos usuários. Os dados coletados por organizações externas, incluindo dados de contato limitados, estão sujeitos às políticas e práticas de privacidade dessas organizações.

## <a name="default-cross-tenant-access-settings"></a>Configurações de acesso entre locatários padrão

As configurações de acesso entre locatários padrão determinam sua postura para colaboração de entrada e saída com todas as outras Azure AD organizações. Qualquer colaboração externa com uma organização não listada explicitamente em suas configurações de acesso entre locatários herdará essas configurações padrão. As configurações padrão são definidas usando o tipo de recurso [crossTenantAccessPolicyConfigurationDefault](../resources/crosstenantaccesspolicyconfigurationdefault.md) .

Por padrão, Azure AD todos os locatários Azure AD uma configuração padrão de serviço para configurações de acesso entre locatários. Você pode substituir esses padrões de serviço por sua própria configuração para se adequar à sua organização. Você pode confirmar se está usando as configurações padrão do serviço ou se modificou as configurações padrão examinando a propriedade **isServiceDefault** retornada quando você consulta o ponto de extremidade padrão.

## <a name="partner-cross-tenant-access-settings"></a>Configurações de acesso entre locatários do parceiro

As configurações de acesso entre locatários específicas do parceiro determinam sua postura para colaboração de entrada e saída com uma organização Azure AD específica. Qualquer colaboração com essa organização herdará essas configurações específicas do parceiro. As configurações de parceiro são definidas usando o tipo de recurso [crossTenantAccessPolicyConfigurationPartner](../resources/crosstenantaccesspolicyconfigurationpartner.md) .

Embora você tenha adicionado um parceiro às suas configurações de acesso entre locatários, algumas das configurações padrão ainda serão aplicadas. Por exemplo, se você configurar apenas **b2bCollaborationInbound** para um parceiro em suas configurações de acesso entre locatários, todas as outras configurações dessa configuração de parceiro serão herdadas das configurações de acesso entre locatários padrão. Ao consultar o ponto de extremidade do parceiro, `null` qualquer propriedade no objeto parceiro significa que, para essa propriedade, ela está herdando configurações da política padrão.

## <a name="inbound-trust-settings-in-cross-tenant-access-settings"></a>Configurações de confiança de entrada nas configurações de acesso entre locatários

As configurações de confiança de entrada permitem que você confie no desempenho dos usuários externos da MFA em seus diretórios base. Isso impede que usuários externos precisem executar a MFA em seus diretórios base e em seu diretório. Com as configurações de confiança de entrada, você habilita uma experiência de autenticação perfeita para seus usuários externos e economiza nos custos de MFA incorridos pela sua organização.  

Por exemplo, quando você define suas configurações de confiança para confiar na MFA, suas políticas de MFA ainda são aplicadas a usuários externos, mas os usuários que já concluiram a MFA em seus locatários domésticos não precisarão concluir a MFA novamente em seu locatário.

As configurações de confiança de entrada também permitem que você confie em dispositivos compatíveis ou Azure AD ingressados em seus diretórios base. Com as configurações de confiança de entrada nas configurações de acesso entre locatários, agora você pode proteger o acesso aos seus aplicativos e recursos exigindo que os usuários externos usem dispositivos ingressados em conformidade ou Azure AD híbridos.

## <a name="interpreting-the-api-response"></a>Interpretando a resposta da API

A API de configurações de acesso entre locatários pode ser usada para configurar várias configurações para permitir ou bloquear o acesso de e para sua organização. A tabela a seguir realça cenários, mostra um exemplo da resposta da API e qual deve ser a interpretação dessa resposta. **b2bSetting** é usado como um espaço reservado para qualquer configuração de entrada B2B (**b2bCollaborationInbound** ou **b2bDirectConnectInbound**) ou de saída (**b2bCollaborationOutbound** ou **b2bDirectConnectOutbound**).

<br/>

<table>
<tr>
<th> Cenário </th> <th> Saída da API </th> <th> Interpretação </th>
</tr>
<tr>
<td> Bloquear todos os usuários e bloquear todos os aplicativos </td>
<td>

``` json
"b2bsetting": {
    "usersAndGroups": {
        "accessType": "blocked",
        "targets": [
            {
                "target": "AllUsers",
                "targetType": "user"
            }
        ]
    },
    "applications": {
        "accessType": "blocked",
        "targets": [
            {
                "target": "AllApplications",
                "targetType": "application"
            }
        ]
    }
}
```

</td>
<td> - </td>
</tr>
<tr>
<td> Permitir todos os usuários e permitir todos os aplicativos </td>
<td>

``` json
"b2bsetting": {
    "usersAndGroups": {
        "accessType": "allowed",
        "targets": [
            {
                "target": "AllUsers",
                "targetType": "user"
            }
        ]
    },
    "applications": {
        "accessType": "allowed",
        "targets": [
            {
                "target": "AllApplications",
                "targetType": "application"
            }
        ]
    }
}
```

</td>
<td> - </td>
</tr>
<tr>
<td> Permitir que os usuários do grupo 'g1' acessem qualquer aplicativo </td>
<td>

``` json
"b2bSetting": {
    "usersAndGroups": {
        "accessType": "allowed",
        "targets": [
            {
                "target": "g1",
                "targetType": "group"
            }
        ]
    },
    "applications": {
        "accessType": "allowed",
        "targets": [
            {
                "target": "AllApplications",
                "targetType": "application"
            }
        ]
    }
}
```

</td>
<td> Os usuários no grupo 'g1' podem acessar qualquer aplicativo. Todos os outros usuários que não estão no grupo 'g1' estão bloqueados. </td>
</tr>
<tr>
<td> Permitir acesso somente ao aplicativo 'a1' </td>
<td>

``` json
"b2bSetting": {
    "usersAndGroups": {
        "accessType": "allowed",
        "targets": [
            {
                "target": "AllUsers",
                "targetType": "user"
            }
        ]
    },
    "applications": {
        "accessType": "allowed",
        "targets": [
            {
                "target": "a1",
                "targetType": "application"
            }
        ]
    }
}
```

</td>
<td> Todos os usuários só têm permissão para acessar o aplicativo 'a1' </td>
</tr>
<tr>
<td> Permitir usuários no grupo 'g1' e bloquear o acesso ao aplicativo 'a1' </td>
<td>

``` json
"b2bSetting": {
    "usersAndGroups": {
        "accessType": "allowed",
        "targets": [
            {
                "target": "g1",
                "targetType": "group"
            }
        ]
    },
    "applications": {
        "accessType": "blocked",
        "targets": [
            {
                "target": "a1",
                "targetType": "application"
            }
        ]
    }
}
```

</td>
<td> Todos os usuários no grupo 'g1' têm permissão para acessar qualquer aplicativo <b>, exceto</b> o aplicativo 'a1'. </td>
</tr>
<tr>
<td> Impedir que os usuários do grupo 'g1' acessem qualquer aplicativo </td>
<td>

``` json
"b2bSetting": {
    "usersAndGroups": {
        "accessType": " blocked",
        "targets": [
            {
                "target": "g1",
                "targetType": "group"
            }
        ]
    },
    "applications": {
        "accessType": "blocked",
        "targets": [
            {
                "target": "AllApplications",
                "targetType": "application"
            }
        ]
    }
}
```

</td>
<td> Os usuários no grupo 'g1' não podem acessar nenhum aplicativo. Outros usuários que não estão no grupo 'g1' têm acesso a todos os aplicativos. </td>
</tr>
<tr>
<td> Bloquear usuários no grupo 'g1' e permitir acesso somente ao aplicativo 'a1' </td>
<td>

``` json
"b2bSetting": {
    "usersAndGroups": {
        "accessType": "blocked",
        "targets": [
            {
                "target": "g1",
                "targetType": "group"
            }
        ]
    },
    "applications": {
        "accessType": "allowed",
        "targets": [
            {
                "target": "a1",
                "targetType": "application"
            }
        ]
    }
}
```

</td>
<td> Os usuários no grupo 'g1' não podem acessar nenhum aplicativo. Qualquer usuário que não estiver no grupo 'g1' só poderá acessar o aplicativo 'a1'. </td>
</tr>
<tr>
<td> Permitir que os usuários do grupo 'g1' acessem somente o aplicativo 'a1' </td>
<td>

``` json
"b2bSetting": {
    "usersAndGroups": {
        "accessType": "allowed",
        "targets": [
            {
                "target": "g1",
                "targetType": "group"
            }
        ]
    },
    "applications": {
        "accessType": "allowed",
        "targets": [
            {
                "target": "a1",
                "targetType": "application"
            }
        ]
    }
}
```

</td>
<td> Os usuários no grupo 'g1' só têm permissão para acessar o aplicativo 'a1'. Todos os usuários, incluindo usuários no grupo 'g1', são impedidos de acessar qualquer outro aplicativo. </td>
</tr>
<tr>
<td> Impedir que os usuários do grupo 'g1' acessem o aplicativo 'a1' </td>
<td>

``` json
"b2bSetting": {
    "usersAndGroups": {
        "accessType": "blocked",
        "targets": [
            {
                "target": "g1",
                "targetType": "group"
            }
        ]
    },
    "applications": {
        "accessType": "blocked",
        "targets": [
            {
                "target": "a1",
                "targetType": "application"
            }
        ]
    }
}
```

</td>
<td> Os usuários no grupo 'g1' são impedidos de acessar somente o aplicativo 'a1'. Todos os usuários, incluindo usuários no grupo 'g1', podem acessar qualquer outro aplicativo. </td>
</tr>
</table>

## <a name="cross-tenant-access-settings-vs-tenant-restrictions"></a>Configurações de acesso entre locatários versus restrições de locatário

Controles de saída de configurações de acesso entre locatários  são para controlar como as contas da sua organização são usadas para acessar recursos em outras Azure AD organizações. As restrições de locatário são para controlar como seus funcionários usam **Azure AD contas de outras organizações enquanto o funcionário está em suas redes ou dispositivos**. De forma crítica, os controles de saída funcionam o tempo todo porque estão associados às suas contas, enquanto as Restrições de Locatário exigem que sinais adicionais sejam injetados nas solicitações de autenticação a serem impostas, pois as Restrições de Locatário estão no escopo de redes e dispositivos, não de contas. Saiba mais sobre [restrições de locatário](/azure/active-directory/manage-apps/tenant-restrictions).

## <a name="next-steps"></a>Próximas etapas

+ [Documentação de configurações de acesso entre locatários](/azure/active-directory/external-identities/cross-tenant-access-overview)
+ [Tipo de recurso crossTenantAccessPolicyConfigurationDefault](../resources/crosstenantaccesspolicyconfigurationdefault.md)
+ [Tipo de recurso crossTenantAccessPolicyConfigurationPartner](../resources/crosstenantaccesspolicyconfigurationpartner.md)
