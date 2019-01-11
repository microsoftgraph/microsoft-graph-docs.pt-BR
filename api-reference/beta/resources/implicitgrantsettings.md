---
title: tipo de recurso de implicitGrantSettings
description: Especifica se esse aplicativo web pode solicitar tokens usando o fluxo de implícita OAuth 2.0. Propriedades separadas estão disponíveis para solicitar tokens de acesso e a ID como parte do fluxo de implícita. Para ativar o fluxo implícito, pelo menos uma das propriedades a seguir deve ser definida como true.
localization_priority: Normal
ms.openlocfilehash: 93a54ac0c0e4c6c32ebb99c9747d44d75f98af07
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834262"
---
# <a name="implicitgrantsettings-resource-type"></a>tipo de recurso de implicitGrantSettings

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Especifica se esse aplicativo web pode solicitar tokens usando o fluxo de implícita OAuth 2.0. Propriedades separadas estão disponíveis para solicitar tokens de acesso e a ID como parte do fluxo de implícita. Para ativar o fluxo implícito, pelo menos uma das propriedades a seguir deve ser definida como true.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------|:-----|:------------|
|enableIdTokenIssuance| Booliano | Especifica se esse aplicativo web pode solicitar um token de ID usando o fluxo de implícita OAuth 2.0.|
|enableAccessTokenIssuance| Booliano | Especifica se esse aplicativo web pode solicitar um token de acesso usando o fluxo de implícita OAuth 2.0.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.

```json
{
  "enableIdTokenIssuance": "Boolean",
  "enableAccessTokenIssuance": "Boolean"
}

```
