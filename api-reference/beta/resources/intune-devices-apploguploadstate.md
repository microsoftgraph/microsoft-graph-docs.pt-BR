---
title: Tipo de número appLogUploadState
description: AppLogUploadStatus
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 7d304c9d0b310d26eb7c4e83144c6fa1e8a9b1b5
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59086278"
---
# <a name="apploguploadstate-enum-type"></a>Tipo de número appLogUploadState

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

AppLogUploadStatus

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|pendente|0|A solicitação está aguardando para ser processada ou em processamento|
|completed|1|A solicitação é concluída com o arquivo carregado no blob do Azure para download.|
|failed|2|Solicitar processamento concluído e em estado de erro.|



