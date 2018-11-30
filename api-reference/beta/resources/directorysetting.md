---
title: tipo de recurso de directorySetting
description: Configurações do diretório podem ser criadas com base no directorySettingTemplates disponíveis e alteradas de seus padrões predefinidos. Essas configurações podem controlar comportamentos de entidade ou recurso, em um nível de locatário todo ou em um nível de entidade específica. Quando a mesma configuração é definida no nível de entidade de todo o inquilino e específicos, a configuração de nível de entidade específica pode recusar da configuração de todo o inquilino.  Por exemplo, a configuração de todo o inquilino pode permitir convidados sejam convidados por membros existentes de grupos, mas uma configuração de grupo específico pode recusar e não permitir convidados sejam convidados por membros do grupo. Atualmente configurações definidas pelo sistema são apenas regem o comportamento de grupos do Office.
ms.openlocfilehash: 4a807d22bfd5d6651b4064542d33fe285b637a3f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036781"
---
# <a name="directorysetting-resource-type"></a>tipo de recurso de directorySetting

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Configurações do diretório podem ser criadas com base no disponíveis [directorySettingTemplates](directorysettingtemplate.md)e alteradas de seus padrões predefinidos. Essas configurações podem controlar comportamentos de entidade ou recurso, em um nível de locatário todo ou em um nível de entidade específica. Quando a mesma configuração é definida no nível de entidade de todo o inquilino e específicos, a configuração de nível de entidade específica pode recusar da configuração de todo o inquilino.  Por exemplo, a configuração de todo o inquilino pode permitir convidados sejam convidados por membros existentes de grupos, mas uma configuração de grupo específico pode recusar e não permitir convidados sejam convidados por membros do grupo. Atualmente configurações definidas pelo sistema são apenas regem o comportamento de grupos do Office.

> **Observação**: A versão /beta do tipo de recurso directorySetting se aplica apenas aos grupos. A versão /v1.0 foi renomeada para groupSetting.

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Criar configuração](../api/directorysetting-post-settings.md) | [directorySetting](directorysetting.md) |Crie um objeto de configuração com base em um directorySettingTemplate. A solicitação POST deve fornecer settingValues para todas as configurações definidas no modelo.|
|[Obter configuração](../api/directorysetting-get.md) | [directorySetting](directorysetting.md) |Ler propriedades de um objeto de configuração específico.|
|[Listar configurações](../api/directorysetting-list.md) | coleção [directorySetting](directorysetting.md) |Lista propriedades de todos os objetos de configuração.|
|[Atualizar configuração](../api/directorysetting-update.md) | [directorySetting](directorysetting.md)  |Atualizar um objeto setting. SettingValues só pode ser alterada em uma atualização.|
|[Excluir configuração](../api/directorysetting-delete.md) | None |Excluir um objeto de configuração. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|displayName|string|Nome de exibição deste grupo de configurações, originado do modelo associado. Somente leitura.|
|id|string| Identificador exclusivo destas configurações. Somente leitura.|
|templateId|string| Identificador exclusivo para o modelo usado para criar este grupo de configurações. Somente leitura.|
|values|conjunto [settingValue](settingvalue.md)| Conjunto de pares de nome/valor. Deve conter e ajustar todas as configurações definidas no modelo.|

## <a name="relationships"></a>Relações
Nenhum


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.directorySetting"
}-->

```json
{
  "displayName": "string",
  "id": "string (identifier)",
  "templateId": "string",
  "values": [{"@odata.type": "microsoft.graph.settingValue"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directorySetting resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->