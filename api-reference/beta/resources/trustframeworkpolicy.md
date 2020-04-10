---
title: trustFrameworkPolicy
description: Na política de estrutura de confiança do Azure AD B2C é chamada de políticas personalizadas. Isso descreve as operações disponíveis em um objeto trustFrameworkPolicy para o locatário.
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 553463811f74a536cd3be5317718e00f91c95260
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/10/2020
ms.locfileid: "43218041"
---
# <a name="trustframeworkpolicy-resource-type"></a>tipo de recurso trustFrameworkPolicy

Namespace: microsoft.graph

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Representa uma diretiva de [estrutura de confiança](/azure/active-directory-b2c/active-directory-b2c-reference-trustframeworks-defined-ief-custom) (também chamada de [política personalizada](/azure/active-directory-b2c/active-directory-b2c-overview-custom)) no [Azure Active Directory B2C](/azure/active-directory-b2c/active-directory-b2c-overview). Uma política de estrutura de confiança fornece controle total sobre as viagens do usuário. Use-o para:

* Personalize as experiências de inscrição e inscrição totalmente.
* Federar para qualquer provedor SAML, Open ID Connect ou OAuth2 Identity Provider.
* Integre-se com outros sistemas ou armazenamentos de dados do usuário chamando pontos de extremidade REST.
* Transforme declarações e personalize tokens emitidos para o aplicativo de terceira parte confiável.

Para obter mais informações, consulte [Custom Policies in Azure Active Directory B2C](/azure/active-directory-b2c/active-directory-b2c-overview-custom).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Criar trustFrameworkPolicy](../api/trustframework-post-trustframeworkpolicy.md)|trustFrameworkPolicy|Criar um novo trustFrameworkPolicy.|
|[Obter trustFrameworkPolicy](../api/trustframeworkpolicy-get.md) |trustFrameworkPolicy|Ler as propriedades de um trustFrameworkPolicy existente.|
|[Listar trustFrameworkPolicies](../api/trustframework-list-trustframeworkpolicies.md)|coleção trustFrameworkPolicy|Listar todos os trustFrameworkPolicies configurados em um locatário.|
|[Atualizar ou criar trustFrameworkPolicy](../api/trustframework-put-trustframeworkpolicy.md)|None|Atualize um trustFrameworkPolicy existente.|
|[Excluir trustFrameworkPolicy](../api/trustframeworkpolicy-delete.md)|None|Excluir um trustFrameworkPolicy existente.|

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

- [trustFrameworkPolicy esquema](/azure/active-directory-b2c/trustframeworkpolicy) para obter informações sobre os elementos do esquema.
- [trustFrameworkPolicy. xsd](https://github.com/Azure-Samples/active-directory-b2c-custom-policy-starterpack/blob/master/TrustFrameworkPolicy_0.3.0.0.xsd)
