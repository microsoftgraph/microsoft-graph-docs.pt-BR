---
title: Visão geral da API de configurações de acesso entre locatários
description: As configurações de acesso entre locatários permitem gerenciar a colaboração B2B e a conexão direta B2B para sua organização.
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
---

# <a name="cross-tenant-access-settings-api-overview"></a>Visão geral da API de configurações de acesso entre locatários

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Na colaboração tradicional do Azure AD B2B, qualquer usuário convidado de uma organização poderia usar sua identidade para acessar recursos em organizações externas. Os administradores não têm controle sobre as identidades dos usuários em seus locatários que têm permissão para entrar em organizações externas. Esses controles limitados dificultam a utilização de identidades da sua organização de maneiras não autorizadas.

**As configurações de acesso entre locatários** permitem controlar e gerenciar a colaboração entre usuários em sua organização e em outras organizações. O controle pode estar no acesso de **saída (como** seus usuários colaboram com outras organizações **), acesso** de entrada (como outras organizações colaboram com você) ou ambos.

Os controles granulares permitem determinar os usuários, grupos e aplicativos, tanto em sua organização quanto em organizações externas, que podem participar da colaboração do Azure AD B2B e da conexão direta do Azure AD B2B. Esses controles são implementados por meio de:

+ **Configurações padrão de acesso entre locatários** que configuram as configurações de acesso de entrada e saída da linha de base.
    + Na colaboração do Azure AD B2B, as duas configurações de acesso são habilitadas por padrão. Isso significa que todos os usuários podem ser convidados para organizações externas e todos os usuários podem convidar usuários externos.
    + No Azure AD B2B conexão direta, as duas configurações de acesso são desabilitadas por padrão.
    + As configurações padrão do serviço podem ser atualizadas.
+ **Configurações de acesso específicas do** parceiro que permitem configurar configurações personalizadas para organizações individuais. Para as organizações configuradas, essa configuração tem precedência sobre as configurações padrão. Portanto, embora a colaboração do Azure AD B2B e a conexão direta do Azure AD B2B possam ser desabilitadas em sua organização por padrão, você pode habilitar esses recursos para uma organização externa específica.

> [!IMPORTANT]
> 
> Ao configurar as configurações de saída de conexão direta B2B, você concorda em permitir que as organizações externas com as que você habilitaram as configurações de saída acessem dados de contato limitados sobre seus usuários. A Microsoft compartilha esses dados com essas organizações para ajudá-las a enviar uma solicitação para se conectar com seus usuários. Os dados coletados por organizações externas, incluindo dados de contato limitados, estão sujeitos às políticas e práticas de privacidade dessas organizações.

## <a name="default-cross-tenant-access-settings"></a>Configurações padrão de acesso entre locatários

As configurações de acesso entre locatários padrão determinam sua posição para colaboração de entrada e saída com todas as outras organizações do Azure AD. Qualquer colaboração externa com uma organização não listada explicitamente em suas configurações de acesso entre locatários herdará essas configurações padrão. As configurações padrão são definidas usando o tipo de recurso [crossTenantAccessPolicyConfigurationDefault](../resources/crosstenantaccesspolicyconfigurationdefault.md) .

Por padrão, o Azure AD atribui a todos os locatários do Azure AD uma configuração padrão de serviço para configurações de acesso entre locatários. Você pode substituir esses padrões de serviço com sua própria configuração para se adequar à sua organização. Você pode confirmar se está usando as configurações padrão do serviço ou modificou as configurações padrão olhando para a **propriedade isServiceDefault** retornada quando você consulta o ponto de extremidade padrão.

## <a name="partner-cross-tenant-access-settings"></a>Configurações de acesso entre locatários do parceiro

As configurações de acesso entre locatários específicas do parceiro determinam sua posição para colaboração de entrada e saída com uma organização específica do Azure AD. Qualquer colaboração com essa organização herdará essas configurações específicas do parceiro. As configurações de parceiro são definidas usando o tipo de recurso [crossTenantAccessPolicyConfigurationPartner](../resources/crosstenantaccesspolicyconfigurationpartner.md) .

Mesmo que você tenha adicionado um parceiro às configurações de acesso entre locatários, algumas das configurações padrão ainda serão aplicadas. Por exemplo, se você configurar apenas **b2bCollaborationInbound** para um parceiro em suas configurações de acesso entre locatários, todas as outras configurações para essa configuração de parceiro serão herdadas das configurações de acesso entre locatários padrão. Ao consultar o ponto de extremidade do parceiro, `null` qualquer propriedade no objeto parceiro significa que, para essa propriedade, ela está herdando configurações da política padrão.

## <a name="inbound-trust-settings-in-cross-tenant-access-settings"></a>Configurações de confiança de entrada em configurações de acesso entre locatários

As configurações de confiança de entrada permitem que você confie nos usuários externos do MFA que executam em seus diretórios internos. Isso impede que os usuários externos tenha que executar o MFA em seus diretórios internos e em seu diretório. Com as configurações de confiança de entrada, você habilita uma experiência de autenticação perfeita para seus usuários externos e economiza nos custos de MFA incorridos pela sua organização.  

Por exemplo, quando você configura suas configurações de confiança para confiar no MFA, suas políticas MFA ainda são aplicadas a usuários externos, mas os usuários que já concluíram o MFA em seus locatários de residência não terão que concluir o MFA novamente em seu locatário.

As configurações de confiança de entrada também permitem que você confie em dispositivos compatíveis ou híbridos que ingressaram no Azure AD em seus diretórios de residência. Com as configurações de confiança de entrada em configurações de acesso entre locatários, agora você pode proteger o acesso aos seus aplicativos e recursos exigindo que usuários externos usem dispositivos ingressados no Azure AD híbridos.

## <a name="interpreting-the-api-response"></a>Interpretando a resposta da API

A API de configurações de acesso entre locatários pode ser usada para configurar várias configurações para permitir ou bloquear o acesso de e para sua organização. A tabela a seguir realça cenários, mostra um exemplo da resposta à API e qual deve ser a interpretação dessa resposta. **b2bSetting** é usado como um espaço reservado para qualquer configuração de entrada B2B (**b2bCollaborationInbound** ou **b2bDirectConnectInbound**) ou de saída (**b2bCollaborationOutbound** ou **b2bDirectConnectOutbound**).

<table>
<tr>
<td> Cenário </td> <td> Saída da API </td> <td> Interpretação </td>
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
<td> Permitir que todos os usuários e permitir todos os aplicativos </td>
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
<td> Os usuários no grupo 'g1' podem acessar qualquer aplicativo. Todos os outros usuários que não estão no grupo 'g1' são bloqueados. </td>
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
<td> Permitir que os usuários no grupo 'g1' e bloquear o acesso ao aplicativo 'a1' </td>
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
<td> Todos os usuários do grupo 'g1' têm permissão para acessar qualquer aplicativo <b>, exceto</b> o aplicativo 'a1'. </td>
</tr>
<tr>
<td> Impedir que usuários no grupo 'g1' acessem qualquer aplicativo </td>
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
<td> Os usuários no grupo 'g1' não podem acessar nenhum aplicativo. Qualquer usuário que não está no grupo 'g1' só pode acessar o aplicativo 'a1'. </td>
</tr>
<tr>
<td> Permitir que os usuários no grupo 'g1' acessem somente o aplicativo 'a1' </td>
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
<td> Os usuários no grupo 'g1' são impedidos de acessar somente o aplicativo 'a1'. Todos os usuários, incluindo usuários no grupo 'g1' são capazes de acessar qualquer outro aplicativo. </td>
</tr>
</table>

## <a name="cross-tenant-access-settings-vs-tenant-restrictions"></a>Configurações de acesso entre locatários versus restrições de locatário

Controles de saída de configurações de acesso entre locatários  são para controlar como as contas da sua organização são usadas para acessar recursos em outras organizações do Azure AD. As restrições de locatários são para controlar como seus funcionários usam contas de outras organizações **do Azure AD enquanto o funcionário está em suas redes ou dispositivos**. De forma crítica, os controles de saída funcionam o tempo todo porque estão associados às suas contas, enquanto as Restrições de Locatário exigem que sinais adicionais sejam injetados nas solicitações de autenticação a serem impostas, pois as Restrições de Locatário são escopo para redes e dispositivos, e não contas. Saiba mais sobre [Restrições de Locatário](/azure/active-directory/manage-apps/tenant-restrictions).

## <a name="next-steps"></a>Próximas etapas

+ [Documentação de configurações de acesso entre locatários](/azure/active-directory/external-identities/cross-tenant-access-overview)
+ [tipo de recurso crossTenantAccessPolicyConfigurationDefault](../resources/crosstenantaccesspolicyconfigurationdefault.md)
+ [Tipo de recurso crossTenantAccessPolicyConfigurationPartner](../resources/crosstenantaccesspolicyconfigurationpartner.md)
