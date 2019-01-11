---
title: tipo de recurso directoryRoleTemplate
description: 'Representa um modelo de função de diretório. Um modelo de função directory Especifica os valores de propriedade de uma função de diretório (directoryRole). Há um objeto de modelo de função de diretório associado para cada uma das funções do diretório que podem ser ativadas em um locatário. Para ler uma função de diretório ou atualizar seus membros, ele deve primeiro ser ativado no inquilino. Por padrão, apenas a função do diretório de administradores de empresa é ativada. Para ativar a outras funções de diretório disponível você enviar uma solicitação POST para o `/directoryRoles` ponto de extremidade com a ID do modelo de função de diretório no qual a função de diretório se baseia especificado no parâmetro **roleTemplateId** da solicitação. Após a conclusão bem-sucedida dessa solicitação, você pode iniciar, em seguida, ler e atribuir membros da função de diretório. **Observação**: um modelo de função de diretório é exposto para a função do diretório de usuários. A função do diretório de usuários é implícita e não é visível para os clientes de diretório. Cada usuário no locatário é atribuído a essa função pela infra-estrutura. A função já está ativada. Não use esse modelo.'
localization_priority: Normal
ms.openlocfilehash: bffff81db3416c538031bce58cfc80580c06f48e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27821186"
---
# <a name="directoryroletemplate-resource-type"></a>tipo de recurso directoryRoleTemplate

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Representa um modelo de função de diretório. Um modelo de função de diretório especifica os valores de propriedade de uma função de diretório ([directoryRole](directoryrole.md)). Há um modelo de função de diretório associado para cada uma das funções de diretório que podem ser ativadas em um locatário. Para ler uma função de diretório ou atualizar seus membros, primeiro ela deve ser ativada no locatário. Apenas a função de diretório Administradores de Empresa é ativada por padrão. Para ativar outras funções de diretório disponíveis, você envia uma solicitação POST para o ponto de extremidade `/directoryRoles` com a ID do modelo de função de diretório no qual se baseia a função directory especificada no parâmetro **roleTemplateId** da solicitação. Após a conclusão bem-sucedida da solicitação, você pode começar a ler e atribuir membros à função de diretório. **Observação**: Um modelo de função de diretório é exposto para a função de diretório Usuários. A função de diretório Users está implícita e não é visível para os clientes de diretório. Todos os usuários do locatário são atribuídos a essa função pela infraestrutura. A função já está ativada. Não use este modelo.


## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Obter directoryRoleTemplate](../api/directoryroletemplate-get.md) | [directoryRoleTemplate](directoryroletemplate.md) |Leia as propriedades e os relacionamentos do objeto directoryRoleTemplate.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|description|String|A descrição definida para a função de diretório. Somente leitura.|
|displayName|String|O nome de exibição para definir para a função de diretório. Somente leitura. |
|id|Cadeia de caracteres|O identificador exclusivo do modelo. Herdado de [directoryObject](directoryobject.md). Você especifica a **id** do modelo de função do diretório para a propriedade **roleTemplateId** na solicitação POST para ativar um [directoryRole](directoryrole.md) em um locatário. Chave, Não anulável. Somente leitura.|

## <a name="relationships"></a>Relações
Nenhum



## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.directoryRoleTemplate"
}-->

```json
{
  "description": "string",
  "displayName": "string",
  "id": "string (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryRoleTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
