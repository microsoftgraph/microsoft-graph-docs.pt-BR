---
title: Tipo denum mobileAppSupersedenceType
description: Indica o tipo de supersedência associado a uma relação entre dois aplicativos móveis.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 91629d4effbda6077eb3c12db62417becbdaf609
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59129058"
---
# <a name="mobileappsupersedencetype-enum-type"></a>Tipo denum mobileAppSupersedenceType

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Indica o tipo de supersedência associado a uma relação entre dois aplicativos móveis.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|update|0|Indica que o aplicativo filho deve ser atualizado pela lógica interna do aplicativo pai.|
|replace|1|Indica que o aplicativo filho deve ser desinstalado antes de instalar o aplicativo pai.|



