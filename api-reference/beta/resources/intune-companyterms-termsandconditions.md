---
title: Tipo de recurso termsAndConditions
description: Conteúdo dos C políticas é apresentado aos usuários após sua primeira tentativa de registrar em Intune e subsequentemente após edições onde um administrador requerido re-aceitação. Eles permitem que os administradores comuniquem as provisões com as quais um usuário deve concordar para que os dispositivos sejam registrados no Intune.
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: aab2ca99726c6e5388dfa5641b19d7c40dd920de
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27965674"
---
# <a name="termsandconditions-resource-type"></a>Tipo de recurso termsAndConditions

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Uma entidade termsAndConditions representa os metadados e conteúdos de determinada política de Termos e Condições (T&C). Os conteúdos das políticas da T&C são apresentados aos usuários na primeira tentativa de registro no Intune, e posteriormente, nas edições em que um administrador solicitou a nova aceitação. Eles permitem que os administradores comuniquem as provisões com as quais um usuário deve concordar para que os dispositivos sejam registrados no Intune.
## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar termsAndConditionses](../api/intune-companyterms-termsandconditions-list.md)|Coleção [termsAndConditions](../resources/intune-companyterms-termsandconditions.md)|Listar propriedades e relações dos objetos [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).|
|[Obter termsAndConditions](../api/intune-companyterms-termsandconditions-get.md)|[termsAndConditions](../resources/intune-companyterms-termsandconditions.md)|Ler propriedades e relações do objeto [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).|
|[Criar termsAndConditions](../api/intune-companyterms-termsandconditions-create.md)|[termsAndConditions](../resources/intune-companyterms-termsandconditions.md)|Criar um novo objeto [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).|
|[Excluir termsAndConditions](../api/intune-companyterms-termsandconditions-delete.md)|Nenhum|Excluir um [termsAndConditions](../resources/intune-companyterms-termsandconditions.md)|
|[Atualizar termsAndConditions](../api/intune-companyterms-termsandconditions-update.md)|[termsAndConditions](../resources/intune-companyterms-termsandconditions.md)|Atualizar as propriedades de um objeto [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Identificador exclusivo da política de T&C.|
|createdDateTime|DateTimeOffset|DateTime em que o objeto foi criado.|
|modifiedDateTime|DateTimeOffset|DateTime da última modificação do objeto.|
|lastModifiedDateTime|DateTimeOffset|DateTime da última modificação do objeto.|
|displayName|Cadeia de caracteres|Nome fornecido pelo administrador para a política de T&C. |
|description|Cadeia de caracteres|Descrição fornecida pelo administrador para a política de T&C.|
|title|Cadeia de caracteres|Título dos termos e condições fornecido pelo administrador. Isso é exibido ao usuário nos prompts de aceitação da política de T&C.|
|bodyText|Cadeia de caracteres|Corpo de texto de termos e condições fornecido pelo administrador, normalmente os termos em si. Isso é exibido ao usuário nos prompts de aceitação da política de T&C.|
|acceptanceStatement|Cadeia de caracteres|Explicação dos termos e condições fornecida pelo administrador, normalmente para descrever o que significa aceitar os termos e condições definidos na política de T&C. Isso é exibido ao usuário nos prompts de aceitação da política de T&C.|
|version|Int32|Inteiro que indica a versão atual dos termos. Incrementado quando um administrador faz uma alteração nos termos e deseja solicitar que os usuários aceitem novamente a política de T&C modificada.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|groupAssignments|coleção [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|A lista de atribuições de grupo para esta diretiva T & C.|
|assignments|Coleção [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md)|A lista de atribuições dessa política de T&C.|
|acceptanceStatuses|Coleção [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)|A lista de status de aceitação dessa política de T&C.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termsAndConditions"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termsAndConditions",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "description": "String",
  "title": "String",
  "bodyText": "String",
  "acceptanceStatement": "String",
  "version": 1024
}
```





