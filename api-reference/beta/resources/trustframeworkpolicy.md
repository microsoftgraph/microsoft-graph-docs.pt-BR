---
title: trustFrameworkPolicy
description: Na política de estrutura de confiança do Azure AD B2C é conhecida como políticas personalizadas. Isso descreve as operações disponíveis em um objeto trustFrameworkPolicy para o locatário.
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: a8bb9fc598613d48ac6b9bb34aa02d24872e6300
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442737"
---
# <a name="trustframeworkpolicy-resource-type"></a>Tipo de recurso trustFrameworkPolicy

Namespace: microsoft.graph

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Representa uma [política da Estrutura de Confiança](/azure/active-directory-b2c/active-directory-b2c-reference-trustframeworks-defined-ief-custom) (também chamada de política [personalizada](/azure/active-directory-b2c/active-directory-b2c-overview-custom)) no [Azure Active Directory B2C](/azure/active-directory-b2c/active-directory-b2c-overview). Uma política da Estrutura de Confiança dá controle total sobre as jornadas do usuário. Use-o para:

* Personalize totalmente as experiências de assinatura e de login.
* Federar para qualquer provedor de identidade SAML, Open ID Connect ou OAuth2.
* Integre-se a outros sistemas ou armazenamentos de dados do usuário chamando pontos de extremidade REST.
* Transforme declarações e personalize tokens emitidos para o aplicativo de terceiros de confiança.

Para obter mais informações, consulte [Políticas personalizadas no Azure Active Directory B2C](/azure/active-directory-b2c/active-directory-b2c-overview-custom).

## <a name="methods"></a>Methods

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Criar trustFrameworkPolicy](../api/trustframework-post-trustframeworkpolicy.md)|trustFrameworkPolicy|Crie um novo trustFrameworkPolicy.|
|[Obter trustFrameworkPolicy](../api/trustframeworkpolicy-get.md) |trustFrameworkPolicy|Ler propriedades de um trustFrameworkPolicy existente.|
|[Listar trustFrameworkPolicies](../api/trustframework-list-trustframeworkpolicies.md)|Coleção trustFrameworkPolicy|Listar todos os trustFrameworkPolicies configurados em um locatário.|
|[Atualizar ou criar trustFrameworkPolicy](../api/trustframework-put-trustframeworkpolicy.md)|Nenhum(a)|Atualize um trustFrameworkPolicy existente.|
|[Excluir trustFrameworkPolicy](../api/trustframeworkpolicy-delete.md)|Nenhum(a)|Exclua um trustFrameworkPolicy existente.|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---------------|:--------|:----------|
|id|String|A ID da política.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "baseType":"microsoft.graph.entity",
  "keyProperty":"id",
  "isMediaEntity":true,
  "@odata.type": "microsoft.graph.trustFrameworkPolicy"
}-->
```json
{
   "id": "B2C_1A_Test"
}
```

## <a name="see-also"></a>Confira também

- [esquema trustFrameworkPolicy](/azure/active-directory-b2c/trustframeworkpolicy) para obter informações sobre os elementos de esquema.
- [trustFrameworkPolicy.xsd](https://github.com/Azure-Samples/active-directory-b2c-custom-policy-starterpack/blob/master/TrustFrameworkPolicy_0.3.0.0.xsd)


