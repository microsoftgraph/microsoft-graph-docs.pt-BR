---
title: Tipo de recurso usageRight
description: Contém informações sobre um usageRight que um usuário/dispositivo atribuiu
author: jeeshnair
localization_priority: Normal
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: d3d7ad0de7eb6929e54b7d3d692c6e562e9da76d
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50130407"
---
# <a name="usageright-resource-type"></a>Tipo de recurso usageRight

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um direito de uso representa uma licença que um usuário ou dispositivo tem para software de terceiros criado em aplicativos de energia ou para assinaturas baseadas em dispositivos (somente dispositivo).

## <a name="methods"></a>Métodos

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar usageRights do usuário](../api/user-list-usagerights.md)|Coleção [usageRight](../resources/usageright.md)|Obter a lista de direitos de uso de um usuário.|
|[Listar usageRights do dispositivo](../api/device-list-usagerights.md)|Coleção [usageRight](../resources/usageright.md)|Obter a lista de direitos de uso de um dispositivo.|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|catalogId|String|ID do produto correspondente ao direito de uso.|
|id|String|A ID do direito de uso.|
|serviceIdentifier|String|Identificador do serviço correspondente ao direito de uso.|
|estado|usageRightState|O estado do direito de uso. Os valores possíveis são: `active`, `inactive`, `warning`, `suspended`.|

### <a name="usagerightstate-values"></a>Valores usageRightState 

| Member             |  Descrição               |
| :----------------- |  :------------------------ |
|ativo              | Indica que o direito de uso está ativo e pode ser usado para benefícios de provisionamento.|
|inativo                | Indica que o direito de uso não está ativo e não pode ser usado para benefícios de provisionamento.|
|warning                | Indica que o direito de uso está em carência provavelmente devido à violação do pagamento. Esse estado pode ser usado para lembrar o pagamento pendente ou oferecer uma experiência degradada.|
|suspended                | Indica que o direito de uso é suspenso provavelmente devido a violação de pagamento|
|unknownFutureValue      | Valor do Sentinel para indicar valores futuros. |

>**Observação:** Somente os estados ativo e de aviso representam um benefício que pode ser usável. Todos os outros estados devem ser tratados como não resultando em um benefício usável.



## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.usageRight",
  "baseType": "",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.usageRight",
  "id": "String (identifier)",
  "catalogId": "String",
  "serviceIdentifier": "String",
  "state": "String"
}
```

