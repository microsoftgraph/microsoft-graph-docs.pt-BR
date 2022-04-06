---
title: Visão geral dos atributos de segurança personalizados usando a API do Microsoft Graph (Visualização)
description: Saiba como definir programaticamente seus próprios atributos de segurança personalizados e atribuí-los a objetos do Azure AD usando a API do Microsoft Graph.
author: rolyon
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: conceptualPageType
ms.openlocfilehash: 609e92333195f883ed8387320f925255654fa5ad
ms.sourcegitcommit: 10719607271380ea56076ccff5a3b774d0005773
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/01/2022
ms.locfileid: "64607754"
---
# <a name="overview-of-custom-security-attributes-using-the-microsoft-graph-api-preview"></a>Visão geral dos atributos de segurança personalizados usando a API do Microsoft Graph (Visualização)

> [!IMPORTANT]
> O recurso de atributos de segurança personalizados está atualmente em Visualização. Consulte Os [Termos de](https://azure.microsoft.com/support/legal/preview-supplemental-terms/) Uso Suplementares para visualizações Microsoft Azure para termos legais que se aplicam aos recursos do Azure que estão em beta, visualização ou que ainda não foram lançados em disponibilidade geral.

[Atributos de](/azure/active-directory/fundamentals/custom-security-attributes-overview) segurança personalizados no Azure Active Directory (Azure AD) são atributos específicos dos negócios (pares de valores-chave) que você pode definir e atribuir a objetos do Azure AD. Esses atributos podem ser usados para armazenar informações, categorizar objetos ou impor o controle de acesso fino sobre recursos específicos do Azure. Atributos de segurança personalizados podem ser usados com o controle de acesso baseado em [atributo do Azure (Azure ABAC)](/azure/role-based-access-control/conditions-overview).

Este artigo fornece uma visão geral de como usar a API do Microsoft Graph para definir e atribuir programaticamente seus próprios atributos de segurança personalizados.

## <a name="key-resource-types"></a>Principais tipos de recursos

A seguir estão os blocos de construção de atributos de segurança personalizados.

### <a name="attribute-sets"></a>Conjuntos de atributos

Um *conjunto de atributos* é um grupo de atributos de segurança personalizados relacionados. Veja a seguir as características gerais dos conjuntos de atributos:

+ O nome não pode incluir espaços ou caracteres especiais.
+ Não é possível renomeá-los ou excluídos.
+ Pode ser delegado a outros usuários para definir e atribuir atributos de segurança personalizados.

Para configurar conjuntos de atributos, use o [tipo de recurso attributeSet](attributeset.md).
 
### <a name="custom-security-attribute-definitions"></a>Definições de atributo de segurança personalizadas

Uma *definição de atributo de segurança personalizada* é o esquema de um atributo de segurança personalizado ou par de valores-chave. Por exemplo, o nome do atributo de segurança personalizado, a descrição, o tipo de dados e os valores predefinidos. A seguir estão as características gerais das definições de atributos de segurança personalizados:

+ O nome não pode incluir espaços ou caracteres especiais.
+ Não pode ser renomeado ou excluído, mas pode ser desativado.
+ Deve fazer parte de um conjunto de atributos.

Para configurar definições de atributo de segurança personalizadas, use o [tipo de recurso customSecurityAttributeDefinition](customsecurityattributedefinition.md).

### <a name="allowed-values"></a>Valores permitidos

*Os valores permitidos* representam os valores predefinidos de um atributo de segurança personalizado. Veja a seguir as características gerais dos valores permitidos:

+ Os valores podem incluir espaços, mas alguns caracteres especiais não são permitidos.
+ Não pode ser renomeado ou excluído, mas pode ser desativado.
+ Mais valores predefinidos podem ser adicionados mais tarde.
+ Pode ser dos tipos de dados Boolean, Integer ou String.

Para configurar valores permitidos, use o [tipo de recurso allowedValue](allowedvalue.md).

## <a name="which-directory-objects-support-custom-security-attributes"></a>Quais objetos de diretório suportam atributos de segurança personalizados?

Atributos de segurança personalizados podem ser atribuídos aos seguintes objetos usando a `customSecurityAttributes` propriedade. Os usuários sincronizados de diretório de um Active Directory local também podem ser atribuídos atributos de segurança personalizados.

+ [user](/graph/api/resources/user?view=graph-rest-beta&preserve-view=true)
+ [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-beta&preserve-view=true)

## <a name="limits-and-constraints"></a>Limites e restrições

Para uma lista dos limites e restrições para atributos de segurança personalizados, consulte [Limites e restrições](/azure/active-directory/fundamentals/custom-security-attributes-overview#limits-and-constraints).

## <a name="permissions"></a>Permissions

Para gerenciar atributos de segurança personalizados, a entidade de chamada deve ser atribuída a uma das seguintes funções do Azure AD. Por padrão, o Administrador Global e outras funções de administrador não têm permissões para ler, definir ou atribuir atributos de segurança personalizados.

+ [Leitor de Definição de Atributo](/azure/active-directory/roles/permissions-reference#attribute-definition-reader)
+ [Administrador de Definição de Atributo](/azure/active-directory/roles/permissions-reference#attribute-definition-administrator)
+ [Leitor de Atribuição de Atributo](/azure/active-directory/roles/permissions-reference#attribute-assignment-reader)
+ [Administrador de Atribuição de Atributo](/azure/active-directory/roles/permissions-reference#attribute-assignment-administrator)

Além disso, a entidade de chamada deve ter as permissões de atributos de [segurança personalizados apropriados](/graph/permissions-reference#custom-security-attributes-permissions).

## <a name="license-requirements"></a>Requisitos de licença

O uso de atributos de segurança personalizados requer uma Azure AD Premium P1 ou uma licença P2.

## <a name="next-steps"></a>Próximas etapas

+ [Tipo de recurso customSecurityAttributeDefinition](/graph/api/resources/customsecurityattributedefinition)
+ [Atribuir, atualizar ou remover atributos de segurança personalizados usando a API Graph Microsoft](/graph/custom-security-attributes-examples)
+ [O que são atributos de segurança personalizados no Azure AD?](/azure/active-directory/fundamentals/custom-security-attributes-overview)

