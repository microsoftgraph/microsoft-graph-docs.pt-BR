---
title: Tipo de recurso synchronizationJob
description: Executa a sincronização periodicamente em segundo plano, sondando alterações em um diretório e as pressionando para outro diretório.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 0f0036cd26a72effba41085d9a4638647fd4060e
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132038"
---
# <a name="synchronizationjob-resource-type"></a>Tipo de recurso synchronizationJob

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Executa a sincronização periodicamente em segundo plano, sondando alterações em um diretório e fazendo com que elas para outro diretório. O trabalho de sincronização é sempre específico para uma instância específica de um aplicativo em seu locatário. Como parte da configuração do trabalho de sincronização, você precisa dar autorização para ler e gravar objetos no diretório de destino e personalizar o esquema de sincronização do trabalho.

## <a name="methods"></a>Métodos

| Método        | Tipo de retorno               | Descrição                  |
|:--------------|:--------------------------|:-----------------------------|
|[List](../api/synchronization-synchronizationjob-list.md)             |[coleção synchronizationJob](synchronization-synchronizationjob.md)  |Listar trabalhos existentes para uma determinada instância de aplicativo (entidade de serviço).|
|[Obter synchronizationJob](../api/synchronization-synchronizationjob-get.md) | [synchronizationJob](synchronization-synchronizationjob.md) |Ler propriedades e relações de um objeto synchronizationJob.|
|[Criar](../api/synchronization-synchronizationjob-post.md)         |[synchronizationJob](synchronization-synchronizationjob.md)   |Crie um novo trabalho para um determinado aplicativo.|
|[Start](../api/synchronization-synchronizationjob-start.md)          |Nenhuma   |Inicie a sincronização. Se o trabalho estiver em um estado pausado, ele continuará do ponto em que o trabalho foi pausado. Se o trabalho estiver em quarentena, o status da quarentena será limpo.|
|[Restart](../api/synchronization-synchronizationjob-restart.md)      |Nenhuma   |Force o trabalho a começar de novo e processe todos os objetos no diretório.|
|[Pause](../api/synchronization-synchronizationjob-pause.md)          |Nenhuma   |Interromper temporariamente a sincronização. Todo o progresso, incluindo o estado do trabalho, persiste, e o trabalho continuará de onde foi deixado quando [uma](../api/synchronization-synchronizationjob-start.md) chamada iniciar é feita.|
|[Delete](../api/synchronization-synchronizationjob-delete.md)        |Nenhuma   |Pare a sincronização e exclua permanentemente todo o estado associado ao trabalho.|
|[Obter synchronizationSchema](../api/synchronization-synchronizationschema-get.md)    |[synchronizationSchema](synchronization-synchronizationschema.md)   |Recupere o esquema de sincronização eficaz do trabalho.|
|[Atualizar synchronizationSchema](../api/synchronization-synchronizationschema-update.md)    |Nenhuma   |Atualize o esquema de sincronização do trabalho. |
|[Validar credenciais](../api/synchronization-synchronizationjob-validatecredentials.md)|Nenhuma|Teste as credenciais fornecidas no diretório de destino.|
|[provisionOnDemand](../api/synchronization-synchronizationjob-provision-on-demand.md)|[Coleção synchronizationJobApplicationParameters](../resources/synchronization-synchronizationjobapplicationparameters.md)|Representa os objetos que serão provisionados e as regras de sincronização executadas. O recurso é usado principalmente para provisionamento sob demanda. |
## <a name="properties"></a>Propriedades

| Propriedade      | Tipo      | Descrição    |
|:--------------|:----------|:---------------|
|id             |String                     |Identificador exclusivo do trabalho de sincronização. Somente leitura.|
|Cronograma       |[synchronizationSchedule](synchronization-synchronizationschedule.md)|Agenda usada para executar o trabalho. Somente leitura.|
|status         |[synchronizationStatus](synchronization-synchronizationstatus.md)     |Status do trabalho, que inclui quando o trabalho foi executado pela última vez, o estado atual do trabalho e erros.|
|synchronizationJobSettings   |[keyValuePair](keyvaluepair.md)    |Configurações associadas ao trabalho. Algumas configurações são herdadas do modelo.|
|templateId     |String    |Identificador do modelo [de sincronização](synchronization-synchronizationtemplate.md) em que esse trabalho se baseia.|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|schema|[synchronizationSchema](synchronization-synchronizationschema.md)| O esquema de sincronização configurado para o trabalho.|

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


