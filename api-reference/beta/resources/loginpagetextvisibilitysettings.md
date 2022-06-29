---
title: Tipo de recurso loginPageTextVisibilitySettings
description: Contém detalhes da identidade visual da organização.
author: AlexanderMars
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 9a18a8678db335b788ef170f97958de5154a1942
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66441717"
---
# <a name="loginpagetextvisibilitysettings-resource-type"></a>Tipo de recurso loginPageTextVisibilitySettings

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa as várias cadeias de caracteres de texto que podem ser ocultadas na página de entrada de um locatário.

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
| hideAccountResetCredentials | Booliano | Opção para ocultar os hiperlinks de redefinição de senha de autoatendimento (SSPR), como "Não é possível acessar sua conta?", "Esqueci minha senha" e "Redefinir agora" no formulário de entrada. |
| hideCannotAccessYourAccount | Booliano | Opção para ocultar a SSPR (redefinição de senha de autoatendimento) "Não é possível acessar sua conta?" hiperlink no formulário de entrada. |
| hideForgotMyPassword | Booliano | Opção para ocultar o hiperlink "Esqueci minha senha" da SSPR (redefinição de senha de autoatendimento) no formulário de entrada. |
| hideResetItNow | Booliano | Opção para ocultar o hiperlink de redefinição de senha de autoatendimento (SSPR) "redefinir agora" no formulário de entrada. |
| hideTermsOfUse | Booliano | Opção para ocultar o hiperlink "Termos de Uso" no rodapé. |
| hidePrivacyAndCookies | Booliano | Opção para ocultar o hiperlink "& Cookies de Privacidade" no rodapé. |

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.loginPageTextVisibilitySettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.loginPageTextVisibilitySettings",
  "hideAccountResetCredentials": "Boolean",
  "hideCannotAccessYourAccount": "Boolean",
  "hideForgotMyPassword": "Boolean",
  "hidePrivacyAndCookies": "Boolean",
  "hideResetItNow": "Boolean",
  "hideTermsOfUse": "Boolean"
}
```
