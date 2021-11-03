---
title: Visão geral dos métodos de autenticação de aplicativos do Azure AD
description: Os métodos de autenticação de aplicativo permitem que os aplicativos adquiram tokens para acessar dados no Azure AD.
ms.localizationpriority: medium
author: madansr7
ms.prod: identity-and-sign-in
doc_type: conceptualPageType
ms.openlocfilehash: 400408b1122feab3a10d951facb0fc40df938052
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60688242"
---
# <a name="azure-ad-application-authentication-methods-api-overview-preview"></a>Visão geral da API dos métodos de autenticação do aplicativo do Azure AD (visualização)

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Métodos de autenticação de aplicativos, como certificados e segredos de senha, permitem que os aplicativos adquiram tokens para acessar dados no Azure Active Directory (Azure AD). As políticas permitem que os administradores de IT imigam práticas recomendadas para como os aplicativos em suas organizações usam esses métodos de autenticação de aplicativos. Por exemplo, um administrador pode configurar uma política para bloquear o uso ou limitar o tempo de vida dos segredos de senha e usar a data de criação do objeto para impor a política.

Essas políticas permitem que as organizações aproveitem os novos recursos de segurança do aplicativo. Ao impor restrições baseadas na data de criação do aplicativo ou entidade de serviço, uma organização pode revisar sua postura atual de segurança do aplicativo, aplicativos de inventário e impor controles de acordo com seus cronogramas e necessidades de resourcing. Essa abordagem usando a data criada permite que a organização aplique a política para novos aplicativos e também a aplique a aplicativos existentes.

Há dois tipos de controles de política:

- Política padrão de locatário que se aplica a todos os aplicativos ou entidades de serviço.
- Políticas de gerenciamento de aplicativo (entidade de serviço ou aplicativo) que permitem a inclusão ou exclusão de aplicativos individuais da política padrão do locatário.

## <a name="tenant-default-app-management-policy"></a>Política de gerenciamento de aplicativo padrão de locatário

Uma política padrão de locatário é um único objeto que sempre existe e é desabilitado por padrão. Ele é definido pelo recurso [tenantAppManagementPolicy](tenantappmanagementpolicy.md) e impõe restrições aos objetos principais do aplicativo versus do serviço. Ele contém as duas propriedades a seguir:

- **applicationRestrictions** permite direcionar aplicativos pertencentes ao locatário (objetos de aplicativo).
- **servicePrincipalRestrictions** permite o direcionamento provisionado de outro locatário (objetos de entidade de serviço.

Essas propriedades permitem que a organização bloqueie aplicativos que se originam dentro de um locatário ou elevam a barra de qualidade para aplicativos provisionados fora do limite do locatário.

## <a name="app-management-policy-for-applications-and-service-principals"></a>Política de gerenciamento de aplicativos para aplicativos e entidades de serviço

As políticas de gerenciamento de aplicativos são definidas no recurso [appManagementPolicy,](appmanagementpolicy.md) que contém uma coleção de políticas com restrições variáveis ou datas de imposição diferentes do que é definido na política padrão do locatário. Uma dessas políticas pode ser atribuída a um aplicativo ou entidade de serviço, excluindo-as da política padrão do locatário.

Quando a política padrão do locatário e uma política de gerenciamento de aplicativos existem, a política de gerenciamento de aplicativos tem precedência e o aplicativo ou entidade de serviço atribuído não herda da política padrão do locatário. Somente uma política pode ser atribuída a um aplicativo ou entidade de serviço.

> [!Note]
> Nem as políticas padrão do locatário nem as políticas de gerenciamento de aplicativo bloqueiam a emissão de tokens para aplicativos existentes. Um aplicativo que não atender aos requisitos de política continuará a funcionar até tentar atualizar o recurso para adicionar um novo segredo.

## <a name="what-restrictions-can-be-managed-in-microsoft-graph"></a>Quais restrições podem ser gerenciadas no Microsoft Graph?

A API de política de métodos de autenticação de aplicativo oferece as seguintes restrições:

| Nome da restrição      | Descrição                                           | Exemplos                                                                                     |
| :--------------- | :---------------------------------------------------- | :------------------------------------------------------------------------------------------- |
| passwordAddition | Restringir segredos de senha em aplicativos completamente. | Bloquear novas senhas em aplicativos criados em ou após '01/01/2019'.                        |
| passwordLifetime | Impor um intervalo máximo de vida útil para um segredo de senha.   | Restrinja todos os novos segredos de senha a no máximo 30 dias para aplicativos criados após 01/01/2015. |
| symmetricKeyAddition | Restringir chaves simétricas em aplicativos. | Bloquear novas chaves simétricas em aplicativos criados em ou após 01/01/2019. |
| symmetricKeyLifetime | Impor um intervalo máximo de vida útil para uma chave simétrica.   | Restrinja todas as novas chaves simétricas a um máximo de 30 dias para aplicativos criados após 01/01/2019. |
| asymmetricKeyLifetime | Impor um intervalo máximo de vida útil para uma chave assimétrica (certificado).   | Restrinja todos os novos segredos de chave assimétricas a no máximo 30 dias para aplicativos criados após 01/01/2019. |

### <a name="single-vs-multi-tenant-apps"></a>Aplicativos single vs multi-tenant

Dependendo de seu aplicativo ser um único locatário ou aplicativo multitenente, você aplicará a política em um aplicativo ou no objeto principal do serviço da seguinte forma:

- Para aplicativos de locatário único, aplique a política ao objeto application.
- Para restringir aplicativos de vários locatários instalados em um locatário do cliente, aplique a política ao objeto application.
- Para restringir aplicativos de vários locatários provisionados de outro locatário, aplique a política ao objeto principal do serviço.

### <a name="summary-of-key-differences-between-the-tenant-default-policy-and-app-management-policies"></a>Resumo das principais diferenças entre a política padrão do locatário e as políticas de gerenciamento de aplicativos

| Política padrão de locatário                                                     | Política de gerenciamento de aplicativos                                                                      |
| ------------------------------------------------------------------ | --------------------------------------------------------------------------------------------------------- |
| A política sempre existe.                                              | Os objetos de política podem ser criados ou atualizados para substituir a política padrão.                                         |
| As restrições são desabilitadas por padrão para app/SP.                   | Permite a personalização para locatário único ou multi locatário(aplicativo de backing em locatários ou aplicativos provisionados).     |
| Permite apenas a definição de objeto de restrição única para todos os recursos.| Permite que vários objetos de política sejam definidos, mas apenas um pode ser aplicado a um recurso.                  |
|Permite a distinção de restrições para objetos de aplicativo versus entidades de serviço. | A política pode ser aplicada a um objeto de entidade de serviço ou aplicativo.                             |
| Aplica todas as restrições configuradas a todos os aplicativos ou entidades de serviço.              |  Aplica apenas as restrições configuradas na política de recurso à entidade de serviço ou aplicativo especificada e não herda da política padrão. |

## <a name="next-steps"></a>Próximas etapas

- [Tipo de recurso tenantAppManagementPolicy.](tenantappmanagementpolicy.md)
- [Tipo de recurso appManagementPolicy.](appmanagementpolicy.md)
