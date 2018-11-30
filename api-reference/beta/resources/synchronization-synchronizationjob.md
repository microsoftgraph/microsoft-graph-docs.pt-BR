---
title: tipo de recurso de synchronizationJob
description: Executa a sincronização por executar periodicamente em segundo plano, sondagem para que as alterações em um diretório e envio-los para um diretório diferente. O trabalho de sincronização sempre é específico para uma determinada instância de um aplicativo no seu locatário. Como parte da configuração do trabalho de sincronização, você precisará fornecer a autorização para ler e gravar objetos em seu diretório de destino e personalize o esquema de sincronização de tarefa.
ms.openlocfilehash: 0e6428f2a088e5326f4412e743489c4d94b10296
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040575"
---
# <a name="synchronizationjob-resource-type"></a>tipo de recurso de synchronizationJob

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Executa a sincronização por executar periodicamente em segundo plano, sondagem para que as alterações em um diretório e envio-los para um diretório diferente. O trabalho de sincronização sempre é específico para uma determinada instância de um aplicativo no seu locatário. Como parte da configuração do trabalho de sincronização, você precisará fornecer a autorização para ler e gravar objetos em seu diretório de destino e personalize o esquema de sincronização de tarefa.

## <a name="methods"></a>Métodos

| Método        | Tipo de retorno               | Descrição                  |
|:--------------|:--------------------------|:-----------------------------|
|[List](../api/synchronization-synchronizationjob-list.md)             |coleção [synchronizationJob](synchronization-synchronizationjob.md)  |Lista os trabalhos existentes para uma instância de determinado aplicativo (entidade de serviço).|
|[Obter synchronizationJob](../api/synchronization-synchronizationjob-get.md) | [synchronizationJob](synchronization-synchronizationjob.md) |Leia as propriedades e os relacionamentos de um objeto synchronizationJob.|
|[Create](../api/synchronization-synchronizationjob-post.md)         |[synchronizationJob](synchronization-synchronizationjob.md)   |Crie um novo trabalho para um determinado aplicativo.|
|[Start](../api/synchronization-synchronizationjob-start.md)          |Nenhum   |Inicie a sincronização. Se o trabalho estiver em um estado pausado, ele continua do ponto onde o trabalho foi pausado. Se o trabalho estiver em quarentena, o status de quarentena está desmarcado.|
|[Restart](../api/synchronization-synchronizationjob-restart.md)      |Nenhum   |Força o trabalho recomece e processar novamente todos os objetos no diretório.|
|[Pause](../api/synchronization-synchronizationjob-pause.md)          |Nenhum   |Interrompa temporariamente a sincronização. Todos o andamento, incluindo o estado do trabalho é persistente e o trabalho continuará de onde ela parou quando uma chamada [Iniciar](../api/synchronization-synchronizationjob-start.md) é feita.|
|[Delete](../api/synchronization-synchronizationjob-delete.md)        |Nenhum   |Parar de sincronização e excluir permanentemente todo o estado associado ao trabalho.|
|[Obter synchrnoizationSchema](../api/synchronization-synchronizationschema-get.md)    |[synchronizationSchema](synchronization-synchronizationschema.md)   |Recupere o esquema de sincronização efetivo do trabalho.|
|[Atualizar synchroizationSchema](../api/synchronization-synchronizationschema-update.md)    |Nenhum   |Atualize esquema de sincronização de tarefa. |
|[Validar as credenciais](../api/synchronization-synchronizationjob-validatecredentials.md)|Nenhum|Teste as credenciais fornecidas com o diretório de destino.|

## <a name="properties"></a>Propriedades

| Propriedade      | Tipo      | Descrição    |
|:--------------|:----------|:---------------|
|id             |String                     |Identificador de trabalho de sincronização exclusivo. Somente leitura.|
|agenda       |[synchronizationSchedule](synchronization-synchronizationschedule.md)|Usada para executar o trabalho de agendamento. Somente leitura.|
|status         |[synchronizationStatus](synchronization-synchronizationstatus.md)     |Status do trabalho, que inclui quando o trabalho foi executado último, o estado atual do trabalho e erros.|
|templateId     |String    |Identificador do [modelo de sincronização](synchronization-synchronizationtemplate.md) em que esse trabalho se baseia.|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|esquema|[synchronizationSchema](synchronization-synchronizationschema.md)| O esquema de sincronização configurado para o trabalho.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationJob"
}-->

```json
{
  "id": "String (identifier)",
  "schedule": {"@odata.type": "microsoft.graph.synchronizationSchedule"},
  "status": {"@odata.type": "microsoft.graph.synchronizationStatus"},
  "templateId": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationJob resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->