---
title: tipo de recurso usageRight
description: Contém informações sobre um usageRight um usuário/dispositivo atribuído
author: jeeshnair
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: e436ad4d793082cbd5c1c8d498b5dbe5b7c7fe54
ms.sourcegitcommit: 2a9b82dae63d8a998711679a379ae1fa89df80e0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/06/2021
ms.locfileid: "60214732"
---
# <a name="usageright-resource-type"></a>tipo de recurso usageRight

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um direito de uso representa uma licença que um usuário ou dispositivo tem para um software de terceiros criado Power Apps ou para assinaturas baseadas em dispositivo (somente dispositivo).

## <a name="methods"></a>Métodos

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar uso do usuárioRights](../api/user-list-usagerights.md)|Coleção [usageRight](../resources/usageright.md)|Obter a lista de direitos de uso de um usuário.|
|[Listar uso do dispositivoRights](../api/device-list-usagerights.md)|Coleção [usageRight](../resources/usageright.md)|Obter a lista de direitos de uso de um dispositivo.|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|catalogId|Cadeia de caracteres|ID do produto correspondente ao direito de uso.|
|id|Cadeia de caracteres|A id do direito de uso.|
|serviceIdentifier|Cadeia de caracteres|Identificador do serviço correspondente ao direito de uso.|
|estado|usageRightState|O estado do direito de uso. Os valores possíveis são: `active`, `inactive`, `warning`, `suspended`.|

### <a name="usagerightstate-values"></a>usageRightState values 

| Member             |  Descrição               |
| :----------------- |  :------------------------ |
|active              | Indica que o direito de uso está ativo e pode ser usado para benefícios de provisionamento.|
|inativo                | Indica que o direito de uso não está ativo e não pode ser usado para benefícios de provisionamento.|
|warning                | Indica que o direito de uso está em boas condições provavelmente devido à violação de pagamento. Esse estado pode ser usado para lembrar o pagamento pendente ou oferecer uma experiência degradada.|
|suspended                | Indica que o direito de uso está suspenso provavelmente devido a violação de pagamento|
|unknownFutureValue      | Valor sentinel para indicar valores futuros. |

>**Observação:** Somente os estados ativos e de aviso representam um benefício usável. Todos os outros estados devem ser tratados como não resultando em um benefício usável.



## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.usageRight",
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

