---
title: Tipo de recurso phoneAuthenticationMethod
description: Uma representação de um telefone registrado para um usuário.
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 397d55050cbe0e985075a83527efff45572afe0b
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50156683"
---
# <a name="phoneauthenticationmethod-resource-type"></a>Tipo de recurso phoneAuthenticationMethod

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Uma representação de um telefone registrado para um usuário. Esse recurso inclui o número de telefone, o tipo de telefone e se o telefone está configurado para o usuário entrar via SMS.

Um telefone tem um dos três tipos: celular, celular alternativo ou escritório. Um usuário pode ter um número registrado para cada tipo e deve ter um telefone celular antes de adicionar um celular alternativo. Ao usar um telefone para a autenticação multifatória (MFA) ou para a redefinição de senha de autoatendente (SSPR), o telefone celular é o padrão e o telefone celular alternativo é o backup. 

Os telefones celulares podem ser usados para sms e chamadas de voz, dependendo das configurações do locatário.

Um telefone de escritório só pode receber chamadas de voz, não mensagens SMS.

A propriedade de estado de login SMS fornece informações sobre se um número de telefone está pronto ou não para entrar via SMS. A seguir estão os valores possíveis.

|Valor|Descrição|
|--------|-----------|
|`notSupported`|Não há suporte para o login principal nesse método de autenticação; por exemplo, a assinatura pode ser habilitada apenas no número de celular principal de um usuário, não no número alternativo.|
|`notAllowedByPolicy`|Esse usuário não está habilitado pela política para usar esse método como uma login principal.|
|`notConfigured`|Esse usuário é habilitado pela política para usar esse método como login principal, mas precisa tomar medidas adicionais para configurá-lo.|
|`phoneNumberNotUnique`|Este usuário tentou configurar um número de telefone como o número principal de login, mas o número não era exclusivo e não pode ser usado como um nome de login.|
|`ready`|Esse método de autenticação está pronto para ser usado na login principal.|

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [List](../api/Authentication-list-phonemethods.md) | [phoneAuthenticationMethod](phoneauthenticationmethod.md) | Leia as propriedades e as relações de todos os objetos phoneAuthenticationMethod desse usuário. |
| [Get](../api/phoneauthenticationmethod-get.md) | [phoneAuthenticationMethod](phoneauthenticationmethod.md) | Leia as propriedades e os relacionamentos do objeto phoneAuthenticationMethod. |
| [Update](../api/phoneauthenticationmethod-update.md) | [phoneAuthenticationMethod](phoneauthenticationmethod.md) | Atualize o objeto phoneAuthenticationMethod. |
| [Delete](../api/phoneauthenticationmethod-delete.md) | Nenhum(a) | Exclua o objeto phoneAuthenticationMethod. |
|[Desabilitar a assinatura de SMS](../api/phoneauthenticationmethod-disablesmssignin.md)|Nenhum(a)|Desativar a login por SMS para um usuário.|
|[Habilitar a assinatura de SMS](../api/phoneauthenticationmethod-enablesmssignin.md)|Nenhum(a)|Ativar a login sms para um usuário.|

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|String| O identificador deste telefone registrado para esse usuário. Somente leitura.|
|phoneNumber|String|O número de telefone para texto ou chamada para autenticação. Os números de telefone usam o formato "+ \<country code\> \<number\> \<extension\> x", com extensão opcional. Por exemplo, +1 5555551234 ou +1 5555551234x123 são válidos. Os números serão rejeitados ao criar/atualizar se não corresponderem ao formato necessário. |
|phoneType|string|O tipo deste telefone. Os valores possíveis `mobile` são: `alternateMobile` , ou `office` .|
|smsSignInState|string|Se um telefone está pronto para ser usado para entrar por SMS ou não. Os valores possíveis `notSupported` são: `notAllowedByPolicy` , , , ou `notEnabled` `phoneNumberNotUnique` `ready` `notConfigured` .|

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


