---
title: Tipo de recurso de usuário
description: Ainda não documentado
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 064fe13e30d578b40bf5b387e8f4da10873bf36e
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59015543"
---
# <a name="user-resource-type"></a>Tipo de recurso de usuário

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ainda não documentado

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar usuários](../api/intune-onboarding-user-list.md)|Coleção [user](../resources/intune-onboarding-user.md)|Listar propriedades e relações de objetos de [user](../resources/intune-onboarding-user.md).|
|[Obter usuário](../api/intune-onboarding-user-get.md)|[user](../resources/intune-onboarding-user.md)|Ler propriedades e relações de objetos de [user](../resources/intune-onboarding-user.md).|
|[Criar usuário](../api/intune-onboarding-user-create.md)|[user](../resources/intune-onboarding-user.md)|Criar um novo objeto de [user](../resources/intune-onboarding-user.md).|
|[Excluir usuário](../api/intune-onboarding-user-delete.md)|Nenhum|Excluir [user](../resources/intune-onboarding-user.md).|
|[Atualizar usuário](../api/intune-onboarding-user-update.md)|[user](../resources/intune-onboarding-user.md)|Atualizar as propriedades de um objeto de [user](../resources/intune-onboarding-user.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Identificador exclusivo do usuário.|
|deviceEnrollmentLimit|Int32|O limite do número máximo de dispositivos que o usuário tem permissão para inscrever. Os valores permitidos vão de 5 a 1000.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.user"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.user",
  "id": "String (identifier)",
  "deviceEnrollmentLimit": 1024
}
```




