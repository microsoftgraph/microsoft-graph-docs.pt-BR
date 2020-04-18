---
title: tipo de recurso phoneAuthenticationMethod
description: Uma representação de um telefone registrado para um usuário.
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 218f4775045009c4168508dbb8678852398df125
ms.sourcegitcommit: 9c16d84eac9c34134864ad63a9bb95c309218a44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/18/2020
ms.locfileid: "43557896"
---
# <a name="phoneauthenticationmethod-resource-type"></a>tipo de recurso phoneAuthenticationMethod

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Uma representação de um telefone registrado para um usuário. Esse recurso inclui o número de telefone, o tipo de telefone e se o telefone está configurado para que o usuário entre via SMS.

Um telefone tem um dos três tipos: móvel, móvel alternativo ou Office. Um usuário pode ter um número registrado para cada tipo e deve ter um telefone celular antes de um telefone celular alternativo ser adicionado. Ao usar um telefone para autenticação multifator (MFA) ou redefinição de senha de autoatendimento (SSPR), o telefone celular é o padrão e o telefone celular alternativo é o backup. 

Telefones móveis podem ser usados para chamadas de voz e SMS, dependendo das configurações do locatário.

Um telefone do Office só pode receber chamadas de voz, não mensagens SMS.

A propriedade de estado de entrada do SMS fornece informações sobre se um número de telefone está pronto para entrar via SMS. Estes são os valores possíveis.

|Valor|Descrição|
|--------|-----------|
|`notSupported`|A entrada principal não é suportada por esse método de autenticação-por exemplo, a entrada pode ser habilitada somente no número de celular principal do usuário, e não no número alternativo.|
|`notAllowedByPolicy`|Este usuário não está habilitado pela política para usar esse método como uma entrada principal.|
|`notConfigured`|Este usuário é habilitado por política para usar esse método como a entrada principal, mas precisa realizar ações adicionais para configurá-lo.|
|`phoneNumberNotUnique`|Este usuário tentou configurar um número de telefone como entrada principal, mas o número não era exclusivo e não pode ser usado como um nome de entrada.|
|`ready`|Este método de autenticação está pronto para uso na entrada principal.|

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [List](../api/Authentication-list-phonemethods.md) | [phoneAuthenticationMethod](phoneauthenticationmethod.md) | Leia as propriedades e as relações de todos os objetos phoneAuthenticationMethod deste usuário. |
| [Get](../api/phoneauthenticationmethod-get.md) | [phoneAuthenticationMethod](phoneauthenticationmethod.md) | Leia as propriedades e os relacionamentos do objeto phoneAuthenticationMethod. |
| [Atualizar](../api/phoneauthenticationmethod-update.md) | [phoneAuthenticationMethod](phoneauthenticationmethod.md) | Atualize o objeto phoneAuthenticationMethod. |
| [Excluir](../api/phoneauthenticationmethod-delete.md) | Nenhuma | Exclua o objeto phoneAuthenticationMethod. |
|[Desabilitar a entrada do SMS](../api/phoneauthenticationmethod-disablesmssignin.md)|Nenhum|Desative a entrada do SMS para um usuário.|
|[Habilitar a entrada do SMS](../api/phoneauthenticationmethod-enablesmssignin.md)|Nenhum|Ative a entrada SMS para um usuário.|

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|String| O identificador desse telefone registrado para este usuário. Somente leitura.|
|phoneNumber|String|O número de telefone para texto ou chamada para autenticação. Os números de telefone usam o formato\<"+\> \<ramal\>\>de\<código de país x", com a extensão opcional. Por exemplo, + 1 5555551234 ou + 1 5555551234x123 são válidas. Os números são rejeitados ao criar/atualizar se não coincidem com o formato necessário. |
|PhoneType|string|O tipo desse telefone. Os valores possíveis são `mobile`: `alternateMobile`,, `office`ou.|
|smsSignInState|string|Se um telefone está pronto para ser usado para entrada do SMS ou não. Os valores possíveis são `notSupported`: `notAllowedByPolicy`, `notEnabled`, `phoneNumberNotUnique`, `ready`, ou `notConfigured`.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.phoneAuthenticationMethod",
  "baseType": "",
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
