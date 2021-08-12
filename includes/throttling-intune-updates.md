---
author: davidmu1
localization_priority: Priority
ms.prod: msgraph
ms.topic: include
ms.openlocfilehash: 2f6c6bb712382e43923de674ee7c27ee182397ba46c34748f1b54b35cd4a5c87
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54196608"
---
<!-- markdownlint-disable MD041 -->
<!-- this file is auto-generated don't edit it manually! -->
#### <a name="intune-updates-service-limits"></a>Limites de serviço de atualização do Intune

| Tipo de solicitação | Limitar por locatário para todos os aplicativos | Limitar por aplicativo por locatário |
| ------------ | ----------------------------- | ------------------------ |
| POST, PUT, DELATE, PATCH | 200 solicitações por 20 segundos | 100 solicitações por 20 segundos |
| Qualquer | 2000 solicitações por 20 segundos | 1000 solicitações por 20 segundos |

Os limites anteriores se aplicam aos seguintes recursos:  
windowsFeatureUpdateCatalogItem, windowsFeatureUpdateProfile, windowsFeatureUpdateProfileAssignment, windowsQualityUpdateCatalogItem, windowsQualityUpdateProfile, windowsQualityUpdateProfileAssignment, windowsUpdateCatalogItem.
