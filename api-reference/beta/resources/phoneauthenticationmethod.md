---
title: Tipo de recurso phoneAuthenticationMethod
description: Uma representação de um telefone registrado para um usuário.
localization_priority: Normal
author: mmcla
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 2d0ec89e21ff6ab7aa39b05acabd81c2b22bd54f
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442898"
---
# <a name="phoneauthenticationmethod-resource-type"></a>Tipo de recurso phoneAuthenticationMethod

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Uma representação de um telefone registrado para um usuário. Esse recurso inclui o número de telefone, o tipo de telefone e se o telefone está configurado para o usuário entrar via SMS.

Um telefone tem um dos três tipos: celular, celular alternativo ou office. Um usuário pode ter um número registrado para cada tipo e deve ter um telefone celular antes que um telefone celular alternativo seja adicionado. Ao usar um telefone para autenticação multifafação (MFA) ou redefinição de senha de autoatendência (SSPR), o telefone celular é o padrão e o telefone celular alternativo é o backup. 

Os telefones celulares podem ser usados para sms e chamadas de voz, dependendo das configurações do locatário.

Um telefone do office só pode receber chamadas de voz, não mensagens SMS.

A propriedade de estado de login SMS fornece informações sobre se um número de telefone está ou não pronto para entrar via SMS. A seguir estão os valores possíveis.

|Valor|Descrição|
|--------|-----------|
|`notSupported`|Não há suporte para entrar primário nesse método de autenticação, por exemplo, a login só pode ser habilitada no número móvel principal de um usuário, não no número alternativo.|
|`notAllowedByPolicy`|Esse usuário não está habilitado pela política para usar esse método como uma assinatura primária.|
|`notConfigured`|Esse usuário está habilitado pela política para usar esse método como login principal, mas precisa tomar medidas adicionais para configurá-lo.|
|`phoneNumberNotUnique`|Esse usuário tentou configurar um número de telefone como login principal, mas o número não era exclusivo e não pode ser usado como um nome de login.|
|`ready`|Esse método de autenticação está pronto para ser usado na login principal.|

## <a name="methods"></a>Methods

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [List](../api/Authentication-list-phonemethods.md) | [phoneAuthenticationMethod](phoneauthenticationmethod.md) | Leia propriedades e relações de todos os objetos phoneAuthenticationMethod deste usuário. |
| [Get](../api/phoneauthenticationmethod-get.md) | [phoneAuthenticationMethod](phoneauthenticationmethod.md) | Ler propriedades e relações do objeto phoneAuthenticationMethod. |
| [Atualização](../api/phoneauthenticationmethod-update.md) | [phoneAuthenticationMethod](phoneauthenticationmethod.md) | Atualizar o objeto phoneAuthenticationMethod. |
| [Delete](../api/phoneauthenticationmethod-delete.md) | Nenhum(a) | Excluir objeto phoneAuthenticationMethod. |
|[Desabilitar a assinatura de SMS](../api/phoneauthenticationmethod-disablesmssignin.md)|Nenhum(a)|Desativar a assinatura SMS para um usuário.|
|[Habilitar a assinatura de SMS](../api/phoneauthenticationmethod-enablesmssignin.md)|Nenhum(a)|Ativar a assinatura SMS para um usuário.|

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|String| O identificador desse telefone registrado para esse usuário. Somente leitura.|
|phoneNumber|String|O número de telefone para texto ou chamada para autenticação. Os números de telefone usam o formato "+ \<country code\> \<number\> \<extension\> x", com a extensão opcional. Por exemplo, +1 5555551234 ou +1 5555551234x123 são válidos. Os números são rejeitados ao criar/atualizar se não corresponderem ao formato necessário. |
|phoneType|string|O tipo deste telefone. Os valores possíveis são: `mobile`, `alternateMobile` ou `office`.|
|smsSignInState|string|Se um telefone está pronto para ser usado para entrar no SMS ou não. Os valores possíveis são: `notSupported` , , , , , ou `notAllowedByPolicy` `notEnabled` `phoneNumberNotUnique` `ready` `notConfigured` .|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.phoneAuthenticationMethod",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "phoneNumber": "String",
  "phoneType": "string",
  "smsSignInState": "string"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "phoneAuthenticationMethod resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


