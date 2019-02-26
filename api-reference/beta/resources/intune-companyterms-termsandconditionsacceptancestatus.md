---
title: Tipo de recurso termsAndConditionsAcceptanceStatus
description: Uma entidade termsAndConditionsAcceptanceStatus representa o status de aceitação de uma política de Termos e Condições (T&C) por um determinado usuário. Os usuários devem aceitar a versão mais recente dos termos para manterem o acesso ao Portal da Empresa.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 35c6c3cd34c21b568f319e6b039856fd1f82ddb4
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30172160"
---
# <a name="termsandconditionsacceptancestatus-resource-type"></a>Tipo de recurso termsAndConditionsAcceptanceStatus

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Uma entidade termsAndConditionsAcceptanceStatus representa o status de aceitação de uma política de Termos e Condições (T&C) por um determinado usuário. Os usuários devem aceitar a versão mais recente dos termos para manterem o acesso ao Portal da Empresa.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar termsAndConditionsAcceptanceStatuses](../api/intune-companyterms-termsandconditionsacceptancestatus-list.md)|Coleção [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)|Lista propriedades e relações do objeto [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).|
|[Obter termsAndConditionsAcceptanceStatus](../api/intune-companyterms-termsandconditionsacceptancestatus-get.md)|[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)|Propriedades de leitura e relações do objeto [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).|
|[Criar termsAndConditionsAcceptanceStatus](../api/intune-companyterms-termsandconditionsacceptancestatus-create.md)|[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)|Cria um novo objeto [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).|
|[Excluir termsAndConditionsAcceptanceStatus](../api/intune-companyterms-termsandconditionsacceptancestatus-delete.md)|Nenhuma|Exclui um [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).|
|[Atualizar termsAndConditionsAcceptanceStatus](../api/intune-companyterms-termsandconditionsacceptancestatus-update.md)|[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)|Atualiza as propriedades de um objeto [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Identificador exclusivo da entidade.|
|userDisplayName|Cadeia de caracteres|Nome de exibição do usuário cuja aceitação a entidade representa.|
|acceptedVersion|Int32|Número da versão mais recente dos T&C aceitos pelo usuário.|
|acceptedDateTime|DateTimeOffset|A data e a hora em que os termos foram aceitos pela última vez pelo usuário.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|termsAndConditions|[termsAndConditions](../resources/intune-companyterms-termsandconditions.md)|Link de navegação para os termos e condições atribuídos.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termsAndConditionsAcceptanceStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
  "id": "String (identifier)",
  "userDisplayName": "String",
  "acceptedVersion": 1024,
  "acceptedDateTime": "String (timestamp)"
}
```




