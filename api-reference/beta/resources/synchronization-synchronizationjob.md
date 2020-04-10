---
title: tipo de recurso synchronizationJob
description: Realiza a sincronização periodicamente em segundo plano, pesquisando alterações em um diretório e empurrando-os para outro diretório.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 18c8076a55643289e8ef33fa4316cd224abfe02e
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/10/2020
ms.locfileid: "43217539"
---
# <a name="synchronizationjob-resource-type"></a>tipo de recurso synchronizationJob

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Realiza a sincronização periodicamente em segundo plano, pesquisando alterações em um diretório e empurrando-os para outro diretório. O trabalho de sincronização é sempre específico para uma instância específica de um aplicativo em seu locatário. Como parte da configuração do trabalho de sincronização, você precisa dar autorização para ler e gravar objetos no diretório de destino e personalizar o esquema de sincronização do trabalho.

## <a name="methods"></a>Métodos

| Método        | Tipo de retorno               | Descrição                  |
|:--------------|:--------------------------|:-----------------------------|
|[List](../api/synchronization-synchronizationjob-list.md)             |coleção [synchronizationJob](synchronization-synchronizationjob.md)  |Listar trabalhos existentes para uma determinada instância de aplicativo (entidade de serviço).|
|[Obter synchronizationJob](../api/synchronization-synchronizationjob-get.md) | [synchronizationJob](synchronization-synchronizationjob.md) |Ler propriedades e relações de um objeto synchronizationJob.|
|[Create](../api/synchronization-synchronizationjob-post.md)         |[synchronizationJob](synchronization-synchronizationjob.md)   |Criar novo trabalho para um determinado aplicativo.|
|[Start](../api/synchronization-synchronizationjob-start.md)          |None   |Inicie a sincronização. Se o trabalho estiver em um estado pausado, ele continuará a partir do ponto em que o trabalho foi pausado. Se o trabalho estiver em quarentena, o status de quarentena será limpo.|
|[Restart](../api/synchronization-synchronizationjob-restart.md)      |None   |Forçar o início do trabalho e processar novamente todos os objetos no diretório.|
|[Pause](../api/synchronization-synchronizationjob-pause.md)          |None   |Interromper temporariamente a sincronização. Todo o progresso, incluindo o estado do trabalho, é mantido e o trabalho continuará de onde parou quando uma chamada [inicial](../api/synchronization-synchronizationjob-start.md) é feita.|
|[Delete](../api/synchronization-synchronizationjob-delete.md)        |None   |Interrompa a sincronização e exclua permanentemente todo o estado associado ao trabalho.|
|[Obter synchronizationSchema](../api/synchronization-synchronizationschema-get.md)    |[synchronizationSchema](synchronization-synchronizationschema.md)   |Recupere o esquema de sincronização efetiva do trabalho.|
|[Atualizar synchronizationSchema](../api/synchronization-synchronizationschema-update.md)    |None   |Atualize o esquema de sincronização do trabalho. |
|[Validar credenciais](../api/synchronization-synchronizationjob-validatecredentials.md)|None|Teste as credenciais fornecidas em relação ao diretório de destino.|

## <a name="properties"></a>Propriedades

| Propriedade      | Tipo      | Descrição    |
|:--------------|:----------|:---------------|
|id             |String                     |Identificador exclusivo do trabalho de sincronização. Somente leitura.|
|Cronograma       |[synchronizationSchedule](synchronization-synchronizationschedule.md)|Agendamento usado para executar o trabalho. Somente leitura.|
|status         |[synchronizationStatus](synchronization-synchronizationstatus.md)     |Status do trabalho, que inclui quando o trabalho foi executado pela última vez, o estado atual do trabalho e os erros.|
|synchronizationJobSettings   |[keyValuePair](keyvaluepair.md)    |Configurações associadas ao trabalho. Algumas configurações são herdadas do modelo.|
|templateId     |Cadeia de Caracteres    |Identificador do [modelo de sincronização](synchronization-synchronizationtemplate.md) em que este trabalho se baseia.|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|esquemas|[synchronizationSchema](synchronization-synchronizationschema.md)| O esquema de sincronização configurado para o trabalho.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.synchronizationJob"
}-->

```json
{
  "id": "String (identifier)",
  "schedule": {"@odata.type": "microsoft.graph.synchronizationSchedule"},
  "status": {"@odata.type": "microsoft.graph.synchronizationStatus"},
  "synchronizationJobSettings": {"@odata.type": "microsoft.graph.keyValuePair"},
  "templateId": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationJob resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
