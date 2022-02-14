---
title: Tipo de recurso loginPageTextVisibilitySettings
description: Contém detalhes da identidade visual da organização.
author: AlexanderMars
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: f31973dad83f09305bdae6a9f9997b6af35d5049
ms.sourcegitcommit: dbacb04ae7138ac3b109683e63a6ff27c166f421
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/14/2022
ms.locfileid: "62805428"
---
# <a name="loginpagetextvisibilitysettings-resource-type"></a>Tipo de recurso loginPageTextVisibilitySettings

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Esse é um tipo complexo que representa os vários textos que podem ser ocultos na página de login de um locatário.

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
| hideCannotAccessYourAccount | Boolean | Opção para ocultar a redefinição de senha de autoatendados (SSPR) "Não é possível acessar sua conta?" hiperlink no formulário de login. |
| hideForgotMyPassword | Boolean | Opção para ocultar o hiperlink de redefinição de senha de autoatendados (SSPR) "Esqueceu minha senha" no formulário de login. |
| hideResetItNow | Boolean | Opção para ocultar o hiperlink de redefinição de senha de autoatendados (SSPR) "redefinir agora" no formulário de login. |
| hideTermsOfUse | Boolean | Opção para ocultar o hiperlink "Termos de Uso" no rodapé. |
| hidePrivacyAndCookies | Boolean | Opção para ocultar o hiperlink "Privacidade & Cookies" no rodapé. |

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
  "hideCannotAccessYourAccount": "Boolean",
  "hideForgotMyPassword": "Boolean",
  "hidePrivacyAndCookies": "Boolean",
  "hideResetItNow": "Boolean",
  "hideTermsOfUse": "Boolean"
}
```
