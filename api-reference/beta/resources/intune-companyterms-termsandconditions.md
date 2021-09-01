---
title: Tipo de recurso termsAndConditions
description: Uma entidade termsAndConditions representa os metadados e conteúdos de determinada política de Termos e Condições (T&C). Os conteúdos das políticas da T&C são apresentados aos usuários na primeira tentativa de registro no Intune, e posteriormente, nas edições em que um administrador solicitou a nova aceitação. Eles permitem que os administradores comuniquem as provisões com as quais um usuário deve concordar para que os dispositivos sejam registrados no Intune.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 723476aa9edaea09ca0bbc916fe63a57a64c3460
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58820517"
---
# <a name="termsandconditions-resource-type"></a>Tipo de recurso termsAndConditions

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

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
|displayName|String|Nome fornecido pelo administrador para a política de T&C. |
|description|String|Descrição fornecida pelo administrador para a política de T&C.|
|title|Cadeia de caracteres|Título dos termos e condições fornecido pelo administrador. Isso é exibido ao usuário nos prompts de aceitação da política de T&C.|
|bodyText|String|Corpo de texto de termos e condições fornecido pelo administrador, normalmente os termos em si. Isso é exibido ao usuário nos prompts de aceitação da política de T&C.|
|acceptanceStatement|String|Explicação dos termos e condições fornecida pelo administrador, normalmente para descrever o que significa aceitar os termos e condições definidos na política de T&C. Isso é exibido ao usuário nos prompts de aceitação da política de T&C.|
|version|Int32|Inteiro que indica a versão atual dos termos. Incrementado quando um administrador faz uma alteração nos termos e deseja solicitar que os usuários aceitem novamente a política de T&C modificada.|
|roleScopeTagIds|Coleção String|Lista de marcas de escopo para esta instância entity.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|groupAssignments|[Coleção termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|A lista de atribuições de grupo para esta política T&C.|
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
  "version": 1024,
  "roleScopeTagIds": [
    "String"
  ]
}
```



