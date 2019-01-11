---
title: Tipo de recurso telecomExpenseManagementPartner
description: Recursos telecomExpenseManagementPartner representam os metadados e o status de um serviço TEM específico. Depois que a sua organização tiver se integrado com um parceiro, este poderá ser habilitado ou desabilitado para ativar ou desativar a funcionalidade TEM.
localization_priority: Normal
ms.openlocfilehash: a0a2f3f3f4bbd0111ec8904c3b4d800da404f19a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27810938"
---
# <a name="telecomexpensemanagementpartner-resource-type"></a>Tipo de recurso telecomExpenseManagementPartner

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Recursos telecomExpenseManagementPartner representam os metadados e o status de um serviço TEM específico. Depois que a sua organização tiver se integrado com um parceiro, este poderá ser habilitado ou desabilitado para ativar ou desativar a funcionalidade TEM.
## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar telecomExpenseManagementPartners](../api/intune-tem-telecomexpensemanagementpartner-list.md)|Coleção [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md)|Lista propriedades e relações dos objetos [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md).|
|[Obter telecomExpenseManagementPartner](../api/intune-tem-telecomexpensemanagementpartner-get.md)|[telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md)|Propriedades de leitura e relações do objeto [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md).|
|[Criar telecomExpenseManagementPartner](../api/intune-tem-telecomexpensemanagementpartner-create.md)|[telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md)|Cria um novo objeto [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md).|
|[Excluir telecomExpenseManagementPartner](../api/intune-tem-telecomexpensemanagementpartner-delete.md)|Nenhuma|Exclui um [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md).|
|[Atualizar telecomExpenseManagementPartner](../api/intune-tem-telecomexpensemanagementpartner-update.md)|[telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md)|Atualiza as propriedades de um objeto [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador exclusivo do parceiro TEM.|
|displayName|Cadeia de caracteres|Nome de exibição do parceiro TEM.|
|url|Cadeia de caracteres|URL do painel de controle administrativo do parceiro TEM, em que um administrador pode configurar o serviço TEM.|
|appAuthorized|Booliano|Se aplicativo AAD do parceiro foi autorizado a acessar o Intune.|
|enabled|Booliano|Se a conexão do Intune com o serviço TEM está habilitada ou desabilitada no momento.|
|lastConnectionDateTime|DateTimeOffset|Carimbo de data/hora da última solicitação enviada ao Intune pelo parceiro TEM.|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.telecomExpenseManagementPartner"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.telecomExpenseManagementPartner",
  "id": "String (identifier)",
  "displayName": "String",
  "url": "String",
  "appAuthorized": true,
  "enabled": true,
  "lastConnectionDateTime": "String (timestamp)"
}
```



