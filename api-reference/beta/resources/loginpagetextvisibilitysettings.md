---
title: Tipo de recurso loginPageTextVisibilitySettings
description: Contém detalhes da identidade visual da organização.
author: AlexanderMars
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: a74e2ea48d8aa39f6e12a6c5c5908d72d445898e
ms.sourcegitcommit: 69b150e408c0b9a0705bf33229269f6e5371bc6c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/07/2022
ms.locfileid: "65924093"
---
# <a name="loginpagetextvisibilitysettings-resource-type"></a>Tipo de recurso loginPageTextVisibilitySettings

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Esse é um tipo complexo que representa os vários textos que podem ser ocultos na página de entrada de um locatário.

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
| hideAccountResetCredentials | Booleano | Opção para ocultar os hiperlinks de redefinição de senha de autoatendimento (SSPR), como "Não é possível acessar sua conta?", "Esqueci minha senha" e "Redefinir agora" no formulário de entrada. |
| hideCannotAccessYourAccount | Booleano | Opção para ocultar a SSPR (redefinição de senha de autoatendimento) "Não é possível acessar sua conta?" hiperlink no formulário de entrada. |
| hideForgotMyPassword | Booleano | Opção para ocultar o hiperlink "Esqueci minha senha" da SSPR (redefinição de senha de autoatendimento) no formulário de entrada. |
| hideResetItNow | Booleano | Opção para ocultar o hiperlink de redefinição de senha de autoatendimento (SSPR) "redefinir agora" no formulário de entrada. |
| hideTermsOfUse | Booleano | Opção para ocultar o hiperlink "Termos de Uso" no rodapé. |
| hidePrivacyAndCookies | Booleano | Opção para ocultar o hiperlink "& Cookies de Privacidade" no rodapé. |

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
