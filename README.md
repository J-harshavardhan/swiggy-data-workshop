[swiggy_workshop_readme.html](https://github.com/user-attachments/files/27116307/swiggy_workshop_readme.html)
<div style="font-family: var(--font-sans); max-width: 680px; padding: 1.5rem 0;">

  <div style="display: flex; align-items: center; gap: 12px; margin-bottom: 6px;">
    <span style="font-size: 28px;">🍔
<div style="font-family: var(--font-sans); max-width: 680px; padding: 1.5rem 0;">

  <div style="display: flex; align-items: center; gap: 12px; margin-bottom: 6px;">
    <span style="font-size: 28px;">🍔</span>
    <div>
      <h1 style="font-size: 22px; font-weight: 500; margin: 0; color: var(--color-text-primary);">Swiggy Orders — Data Analysis Workshop</h1>
      <p style="font-size: 14px; color: var(--color-text-secondary); margin: 4px 0 0;">A hands-on Python workshop using a simulated Swiggy dataset</p>
    </div>
  </div>

  <div style="display: flex; gap: 8px; margin: 16px 0 24px; flex-wrap: wrap;">
    <span style="background: #E6F1FB; color: #0C447C; font-size: 12px; padding: 3px 10px; border-radius: 20px;">Python</span>
    <span style="background: #EAF3DE; color: #3B6D11; font-size: 12px; padding: 3px 10px; border-radius: 20px;">Pandas</span>
    <span style="background: #EEEDFE; color: #3C3489; font-size: 12px; padding: 3px 10px; border-radius: 20px;">NumPy</span>
    <span style="background: #FAEEDA; color: #633806; font-size: 12px; padding: 3px 10px; border-radius: 20px;">Jupyter</span>
    <span style="background: #E1F5EE; color: #085041; font-size: 12px; padding: 3px 10px; border-radius: 20px;">2,050 rows</span>
  </div>

  <div style="background: var(--color-background-secondary); border-radius: var(--border-radius-lg); padding: 1rem 1.25rem; margin-bottom: 24px; font-family: var(--font-mono); font-size: 13px; color: var(--color-text-secondary);">
    <div style="margin-bottom: 4px;">📁 swiggy-data-workshop/</div>
    <div style="margin-left: 16px; margin-bottom: 2px;">├── Swiggy_Workshop.ipynb &nbsp;<span style="color: var(--color-text-tertiary);"># main notebook</span></div>
    <div style="margin-left: 16px; margin-bottom: 2px;">├── swiggy_orders.csv &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: var(--color-text-tertiary);"># raw dataset</span></div>
    <div style="margin-left: 16px; margin-bottom: 2px;">├── swiggy_orders_clean.csv <span style="color: var(--color-text-tertiary);"># cleaned output</span></div>
    <div style="margin-left: 16px;">└── README.md</div>
  </div>

  <h2 style="font-size: 16px; font-weight: 500; margin: 0 0 12px; color: var(--color-text-primary);">Key metrics</h2>
  <div style="display: grid; grid-template-columns: repeat(3, minmax(0, 1fr)); gap: 10px; margin-bottom: 24px;">
    <div style="background: #EEEDFE; border-radius: var(--border-radius-md); padding: 12px 14px;">
      <div style="font-size: 11px; color: #534AB7; margin-bottom: 4px;">GMV</div>
      <div style="font-size: 14px; font-weight: 500; color: #3C3489;">sum(order_value)</div>
      <div style="font-size: 11px; color: #534AB7; margin-top: 4px;">Total platform revenue</div>
    </div>
    <div style="background: #E1F5EE; border-radius: var(--border-radius-md); padding: 12px 14px;">
      <div style="font-size: 11px; color: #0F6E56; margin-bottom: 4px;">AOV</div>
      <div style="font-size: 14px; font-weight: 500; color: #085041;">GMV / orders</div>
      <div style="font-size: 11px; color: #0F6E56; margin-top: 4px;">Avg spend per order</div>
    </div>
    <div style="background: #FAEEDA; border-radius: var(--border-radius-md); padding: 12px 14px;">
      <div style="font-size: 11px; color: #854F0B; margin-bottom: 4px;">Whale orders</div>
      <div style="font-size: 14px; font-weight: 500; color: #633806;">≥ ₹1,000</div>
      <div style="font-size: 11px; color: #854F0B; margin-top: 4px;">Top 5% spenders</div>
    </div>
  </div>

  <h2 style="font-size: 16px; font-weight: 500; margin: 0 0 12px; color: var(--color-text-primary);">Workshop sections</h2>
  <div style="display: flex; flex-direction: column; gap: 8px; margin-bottom: 24px;">
    <div style="background: var(--color-background-primary); border: 0.5px solid var(--color-border-tertiary); border-radius: var(--border-radius-lg); padding: 12px 16px; display: flex; gap: 12px; align-items: flex-start;">
      <span style="background: #EEEDFE; color: #3C3489; font-size: 12px; font-weight: 500; padding: 2px 8px; border-radius: 20px; white-space: nowrap; margin-top: 1px;">1</span>
      <div>
        <div style="font-size: 14px; font-weight: 500; color: var(--color-text-primary); margin-bottom: 2px;">NumPy arrays & vectorised operations</div>
        <div style="font-size: 13px; color: var(--color-text-secondary);">GMV, AOV, percentiles · revenue tier segmentation (Micro / Mid / Premium / Whale)</div>
      </div>
    </div>
    <div style="background: var(--color-background-primary); border: 0.5px solid var(--color-border-tertiary); border-radius: var(--border-radius-lg); padding: 12px 16px; display: flex; gap: 12px; align-items: flex-start;">
      <span style="background: #E1F5EE; color: #085041; font-size: 12px; font-weight: 500; padding: 2px 8px; border-radius: 20px; white-space: nowrap; margin-top: 1px;">2</span>
      <div>
        <div style="font-size: 14px; font-weight: 500; color: var(--color-text-primary); margin-bottom: 2px;">Load & inspect real datasets</div>
        <div style="font-size: 13px; color: var(--color-text-secondary);">dtypes · .info() · .describe() · anomaly detection (bad ratings, negative delivery times)</div>
      </div>
    </div>
    <div style="background: var(--color-background-primary); border: 0.5px solid var(--color-border-tertiary); border-radius: var(--border-radius-lg); padding: 12px 16px; display: flex; gap: 12px; align-items: flex-start;">
      <span style="background: #E6F1FB; color: #0C447C; font-size: 12px; font-weight: 500; padding: 2px 8px; border-radius: 20px; white-space: nowrap; margin-top: 1px;">3</span>
      <div>
        <div style="font-size: 14px; font-weight: 500; color: var(--color-text-primary); margin-bottom: 2px;">Filter, sort & slice</div>
        <div style="font-size: 13px; color: var(--color-text-secondary);">Boolean masks · .loc vs .iloc · top restaurants · loyal dinner crowd segment</div>
      </div>
    </div>
    <div style="background: var(--color-background-primary); border: 0.5px solid var(--color-border-tertiary); border-radius: var(--border-radius-lg); padding: 12px 16px; display: flex; gap: 12px; align-items: flex-start;">
      <span style="background: #FAEEDA; color: #633806; font-size: 12px; font-weight: 500; padding: 2px 8px; border-radius: 20px; white-space: nowrap; margin-top: 1px;">4</span>
      <div>
        <div style="font-size: 14px; font-weight: 500; color: var(--color-text-primary); margin-bottom: 2px;">GroupBy & aggregations</div>
        <div style="font-size: 13px; color: var(--color-text-secondary);">City GMV · category × time slot matrix · pivot tables · .transform() for % share</div>
      </div>
    </div>
    <div style="background: var(--color-background-primary); border: 0.5px solid var(--color-border-tertiary); border-radius: var(--border-radius-lg); padding: 12px 16px; display: flex; gap: 12px; align-items: flex-start;">
      <span style="background: #FCEBEB; color: #791F1F; font-size: 12px; font-weight: 500; padding: 2px 8px; border-radius: 20px; white-space: nowrap; margin-top: 1px;">5</span>
      <div>
        <div style="font-size: 14px; font-weight: 500; color: var(--color-text-primary); margin-bottom: 2px;">Nulls, duplicates & dirty data</div>
        <div style="font-size: 13px; color: var(--color-text-secondary);">Null audit · fix bad values · deduplication · 3σ outlier detection · export clean CSV</div>
      </div>
    </div>
  </div>

  <h2 style="font-size: 16px; font-weight: 500; margin: 0 0 12px; color: var(--color-text-primary);">Dataset columns</h2>
  <div style="display: grid; grid-template-columns: repeat(2, minmax(0,1fr)); gap: 6px; margin-bottom: 24px;">
    <div style="font-size: 12px; padding: 6px 10px; background: var(--color-background-secondary); border-radius: var(--border-radius-md); display: flex; justify-content: space-between;"><span style="font-family: var(--font-mono); color: var(--color-text-primary);">order_id</span><span style="color: var(--color-text-tertiary);">int · ⚠️ dupes</span></div>
    <div style="font-size: 12px; padding: 6px 10px; background: var(--color-background-secondary); border-radius: var(--border-radius-md); display: flex; justify-content: space-between;"><span style="font-family: var(--font-mono); color: var(--color-text-primary);">restaurant_name</span><span style="color: var(--color-text-tertiary);">str</span></div>
    <div style="font-size: 12px; padding: 6px 10px; background: var(--color-background-secondary); border-radius: var(--border-radius-md); display: flex; justify-content: space-between;"><span style="font-family: var(--font-mono); color: var(--color-text-primary);">city</span><span style="color: var(--color-text-tertiary);">str · 12 cities</span></div>
    <div style="font-size: 12px; padding: 6px 10px; background: var(--color-background-secondary); border-radius: var(--border-radius-md); display: flex; justify-content: space-between;"><span style="font-family: var(--font-mono); color: var(--color-text-primary);">category</span><span style="color: var(--color-text-tertiary);">str</span></div>
    <div style="font-size: 12px; padding: 6px 10px; background: var(--color-background-secondary); border-radius: var(--border-radius-md); display: flex; justify-content: space-between;"><span style="font-family: var(--font-mono); color: var(--color-text-primary);">order_value</span><span style="color: var(--color-text-tertiary);">float · ₹</span></div>
    <div style="font-size: 12px; padding: 6px 10px; background: var(--color-background-secondary); border-radius: var(--border-radius-md); display: flex; justify-content: space-between;"><span style="font-family: var(--font-mono); color: var(--color-text-primary);">delivery_time_mins</span><span style="color: var(--color-text-tertiary);">int · ⚠️ nulls/neg</span></div>
    <div style="font-size: 12px; padding: 6px 10px; background: var(--color-background-secondary); border-radius: var(--border-radius-md); display: flex; justify-content: space-between;"><span style="font-family: var(--font-mono); color: var(--color-text-primary);">rating</span><span style="color: var(--color-text-tertiary);">float · ⚠️ nulls/>5</span></div>
    <div style="font-size: 12px; padding: 6px 10px; background: var(--color-background-secondary); border-radius: var(--border-radius-md); display: flex; justify-content: space-between;"><span style="font-family: var(--font-mono); color: var(--color-text-primary);">order_date</span><span style="color: var(--color-text-tertiary);">datetime</span></div>
    <div style="font-size: 12px; padding: 6px 10px; background: var(--color-background-secondary); border-radius: var(--border-radius-md); display: flex; justify-content: space-between;"><span style="font-family: var(--font-mono); color: var(--color-text-primary);">time_slot</span><span style="color: var(--color-text-tertiary);">breakfast/lunch/…</span></div>
    <div style="font-size: 12px; padding: 6px 10px; background: var(--color-background-secondary); border-radius: var(--border-radius-md); display: flex; justify-content: space-between;"><span style="font-family: var(--font-mono); color: var(--color-text-primary);">is_reorder</span><span style="color: var(--color-text-tertiary);">bool</span></div>
    <div style="font-size: 12px; padding: 6px 10px; background: var(--color-background-secondary); border-radius: var(--border-radius-md); display: flex; justify-content: space-between;"><span style="font-family: var(--font-mono); color: var(--color-text-primary);">discount_applied</span><span style="color: var(--color-text-tertiary);">float · NaN=none</span></div>
    <div style="font-size: 12px; padding: 6px 10px; background: var(--color-background-secondary); border-radius: var(--border-radius-md); display: flex; justify-content: space-between;"><span style="font-family: var(--font-mono); color: var(--color-text-primary);">platform</span><span style="color: var(--color-text-tertiary);">iOS/Android/Web</span></div>
  </div>

  <h2 style="font-size: 16px; font-weight: 500; margin: 0 0 10px; color: var(--color-text-primary);">Getting started</h2>
  <div style="background: var(--color-background-secondary); border-radius: var(--border-radius-lg); padding: 1rem 1.25rem; font-family: var(--font-mono); font-size: 13px; color: var(--color-text-secondary); margin-bottom: 24px; line-height: 1.9;">
    <div>pip install numpy pandas jupyter</div>
    <div>git clone https://github.com/J-harshavardhan/swiggy-data-workshop.git</div>
    <div>cd swiggy-data-workshop</div>
    <div>jupyter notebook Swiggy_Workshop.ipynb</div>
  </div>

  <div style="border-top: 0.5px solid var(--color-border-tertiary); padding-top: 14px; font-size: 12px; color: var(--color-text-tertiary);">
    Educational purposes only · Dataset is synthetically generated
  </div>
</div>
</span>
    <div>
      <h1 style="font-size: 22px; font-weight: 500; margin: 0; color: var(--color-text-primary);">Swiggy Orders — Data Analysis Workshop</h1>
      <p style="font-size: 14px; color: var(--color-text-secondary); margin: 4px 0 0;">A hands-on Python workshop using a simulated Swiggy dataset</p>
    </div>
  </div>

  <div style="display: flex; gap: 8px; margin: 16px 0 24px; flex-wrap: wrap;">
    <span style="background: #E6F1FB; color: #0C447C; font-size: 12px; padding: 3px 10px; border-radius: 20px;">Python</span>
    <span style="background: #EAF3DE; color: #3B6D11; font-size: 12px; padding: 3px 10px; border-radius: 20px;">Pandas</span>
    <span style="background: #EEEDFE; color: #3C3489; font-size: 12px; padding: 3px 10px; border-radius: 20px;">NumPy</span>
    <span style="background: #FAEEDA; color: #633806; font-size: 12px; padding: 3px 10px; border-radius: 20px;">Jupyter</span>
    <span style="background: #E1F5EE; color: #085041; font-size: 12px; padding: 3px 10px; border-radius: 20px;">2,050 rows</span>
  </div>

  <div style="background: var(--color-background-secondary); border-radius: var(--border-radius-lg); padding: 1rem 1.25rem; margin-bottom: 24px; font-family: var(--font-mono); font-size: 13px; color: var(--color-text-secondary);">
    <div style="margin-bottom: 4px;">📁 swiggy-data-workshop/</div>
    <div style="margin-left: 16px; margin-bottom: 2px;">├── Swiggy_Workshop.ipynb &nbsp;<span style="color: var(--color-text-tertiary);"># main notebook</span></div>
    <div style="margin-left: 16px; margin-bottom: 2px;">├── swiggy_orders.csv &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: var(--color-text-tertiary);"># raw dataset</span></div>
    <div style="margin-left: 16px; margin-bottom: 2px;">├── swiggy_orders_clean.csv <span style="color: var(--color-text-tertiary);"># cleaned output</span></div>
    <div style="margin-left: 16px;">└── README.md</div>
  </div>

  <h2 style="font-size: 16px; font-weight: 500; margin: 0 0 12px; color: var(--color-text-primary);">Key metrics</h2>
  <div style="display: grid; grid-template-columns: repeat(3, minmax(0, 1fr)); gap: 10px; margin-bottom: 24px;">
    <div style="background: #EEEDFE; border-radius: var(--border-radius-md); padding: 12px 14px;">
      <div style="font-size: 11px; color: #534AB7; margin-bottom: 4px;">GMV</div>
      <div style="font-size: 14px; font-weight: 500; color: #3C3489;">sum(order_value)</div>
      <div style="font-size: 11px; color: #534AB7; margin-top: 4px;">Total platform revenue</div>
    </div>
    <div style="background: #E1F5EE; border-radius: var(--border-radius-md); padding: 12px 14px;">
      <div style="font-size: 11px; color: #0F6E56; margin-bottom: 4px;">AOV</div>
      <div style="font-size: 14px; font-weight: 500; color: #085041;">GMV / orders</div>
      <div style="font-size: 11px; color: #0F6E56; margin-top: 4px;">Avg spend per order</div>
    </div>
    <div style="background: #FAEEDA; border-radius: var(--border-radius-md); padding: 12px 14px;">
      <div style="font-size: 11px; color: #854F0B; margin-bottom: 4px;">Whale orders</div>
      <div style="font-size: 14px; font-weight: 500; color: #633806;">≥ ₹1,000</div>
      <div style="font-size: 11px; color: #854F0B; margin-top: 4px;">Top 5% spenders</div>
    </div>
  </div>

  <h2 style="font-size: 16px; font-weight: 500; margin: 0 0 12px; color: var(--color-text-primary);">Workshop sections</h2>
  <div style="display: flex; flex-direction: column; gap: 8px; margin-bottom: 24px;">
    <div style="background: var(--color-background-primary); border: 0.5px solid var(--color-border-tertiary); border-radius: var(--border-radius-lg); padding: 12px 16px; display: flex; gap: 12px; align-items: flex-start;">
      <span style="background: #EEEDFE; color: #3C3489; font-size: 12px; font-weight: 500; padding: 2px 8px; border-radius: 20px; white-space: nowrap; margin-top: 1px;">1</span>
      <div>
        <div style="font-size: 14px; font-weight: 500; color: var(--color-text-primary); margin-bottom: 2px;">NumPy arrays & vectorised operations</div>
        <div style="font-size: 13px; color: var(--color-text-secondary);">GMV, AOV, percentiles · revenue tier segmentation (Micro / Mid / Premium / Whale)</div>
      </div>
    </div>
    <div style="background: var(--color-background-primary); border: 0.5px solid var(--color-border-tertiary); border-radius: var(--border-radius-lg); padding: 12px 16px; display: flex; gap: 12px; align-items: flex-start;">
      <span style="background: #E1F5EE; color: #085041; font-size: 12px; font-weight: 500; padding: 2px 8px; border-radius: 20px; white-space: nowrap; margin-top: 1px;">2</span>
      <div>
        <div style="font-size: 14px; font-weight: 500; color: var(--color-text-primary); margin-bottom: 2px;">Load & inspect real datasets</div>
        <div style="font-size: 13px; color: var(--color-text-secondary);">dtypes · .info() · .describe() · anomaly detection (bad ratings, negative delivery times)</div>
      </div>
    </div>
    <div style="background: var(--color-background-primary); border: 0.5px solid var(--color-border-tertiary); border-radius: var(--border-radius-lg); padding: 12px 16px; display: flex; gap: 12px; align-items: flex-start;">
      <span style="background: #E6F1FB; color: #0C447C; font-size: 12px; font-weight: 500; padding: 2px 8px; border-radius: 20px; white-space: nowrap; margin-top: 1px;">3</span>
      <div>
        <div style="font-size: 14px; font-weight: 500; color: var(--color-text-primary); margin-bottom: 2px;">Filter, sort & slice</div>
        <div style="font-size: 13px; color: var(--color-text-secondary);">Boolean masks · .loc vs .iloc · top restaurants · loyal dinner crowd segment</div>
      </div>
    </div>
    <div style="background: var(--color-background-primary); border: 0.5px solid var(--color-border-tertiary); border-radius: var(--border-radius-lg); padding: 12px 16px; display: flex; gap: 12px; align-items: flex-start;">
      <span style="background: #FAEEDA; color: #633806; font-size: 12px; font-weight: 500; padding: 2px 8px; border-radius: 20px; white-space: nowrap; margin-top: 1px;">4</span>
      <div>
        <div style="font-size: 14px; font-weight: 500; color: var(--color-text-primary); margin-bottom: 2px;">GroupBy & aggregations</div>
        <div style="font-size: 13px; color: var(--color-text-secondary);">City GMV · category × time slot matrix · pivot tables · .transform() for % share</div>
      </div>
    </div>
    <div style="background: var(--color-background-primary); border: 0.5px solid var(--color-border-tertiary); border-radius: var(--border-radius-lg); padding: 12px 16px; display: flex; gap: 12px; align-items: flex-start;">
      <span style="background: #FCEBEB; color: #791F1F; font-size: 12px; font-weight: 500; padding: 2px 8px; border-radius: 20px; white-space: nowrap; margin-top: 1px;">5</span>
      <div>
        <div style="font-size: 14px; font-weight: 500; color: var(--color-text-primary); margin-bottom: 2px;">Nulls, duplicates & dirty data</div>
        <div style="font-size: 13px; color: var(--color-text-secondary);">Null audit · fix bad values · deduplication · 3σ outlier detection · export clean CSV</div>
      </div>
    </div>
  </div>

  <h2 style="font-size: 16px; font-weight: 500; margin: 0 0 12px; color: var(--color-text-primary);">Dataset columns</h2>
  <div style="display: grid; grid-template-columns: repeat(2, minmax(0,1fr)); gap: 6px; margin-bottom: 24px;">
    <div style="font-size: 12px; padding: 6px 10px; background: var(--color-background-secondary); border-radius: var(--border-radius-md); display: flex; justify-content: space-between;"><span style="font-family: var(--font-mono); color: var(--color-text-primary);">order_id</span><span style="color: var(--color-text-tertiary);">int · ⚠️ dupes</span></div>
    <div style="font-size: 12px; padding: 6px 10px; background: var(--color-background-secondary); border-radius: var(--border-radius-md); display: flex; justify-content: space-between;"><span style="font-family: var(--font-mono); color: var(--color-text-primary);">restaurant_name</span><span style="color: var(--color-text-tertiary);">str</span></div>
    <div style="font-size: 12px; padding: 6px 10px; background: var(--color-background-secondary); border-radius: var(--border-radius-md); display: flex; justify-content: space-between;"><span style="font-family: var(--font-mono); color: var(--color-text-primary);">city</span><span style="color: var(--color-text-tertiary);">str · 12 cities</span></div>
    <div style="font-size: 12px; padding: 6px 10px; background: var(--color-background-secondary); border-radius: var(--border-radius-md); display: flex; justify-content: space-between;"><span style="font-family: var(--font-mono); color: var(--color-text-primary);">category</span><span style="color: var(--color-text-tertiary);">str</span></div>
    <div style="font-size: 12px; padding: 6px 10px; background: var(--color-background-secondary); border-radius: var(--border-radius-md); display: flex; justify-content: space-between;"><span style="font-family: var(--font-mono); color: var(--color-text-primary);">order_value</span><span style="color: var(--color-text-tertiary);">float · ₹</span></div>
    <div style="font-size: 12px; padding: 6px 10px; background: var(--color-background-secondary); border-radius: var(--border-radius-md); display: flex; justify-content: space-between;"><span style="font-family: var(--font-mono); color: var(--color-text-primary);">delivery_time_mins</span><span style="color: var(--color-text-tertiary);">int · ⚠️ nulls/neg</span></div>
    <div style="font-size: 12px; padding: 6px 10px; background: var(--color-background-secondary); border-radius: var(--border-radius-md); display: flex; justify-content: space-between;"><span style="font-family: var(--font-mono); color: var(--color-text-primary);">rating</span><span style="color: var(--color-text-tertiary);">float · ⚠️ nulls/>5</span></div>
    <div style="font-size: 12px; padding: 6px 10px; background: var(--color-background-secondary); border-radius: var(--border-radius-md); display: flex; justify-content: space-between;"><span style="font-family: var(--font-mono); color: var(--color-text-primary);">order_date</span><span style="color: var(--color-text-tertiary);">datetime</span></div>
    <div style="font-size: 12px; padding: 6px 10px; background: var(--color-background-secondary); border-radius: var(--border-radius-md); display: flex; justify-content: space-between;"><span style="font-family: var(--font-mono); color: var(--color-text-primary);">time_slot</span><span style="color: var(--color-text-tertiary);">breakfast/lunch/…</span></div>
    <div style="font-size: 12px; padding: 6px 10px; background: var(--color-background-secondary); border-radius: var(--border-radius-md); display: flex; justify-content: space-between;"><span style="font-family: var(--font-mono); color: var(--color-text-primary);">is_reorder</span><span style="color: var(--color-text-tertiary);">bool</span></div>
    <div style="font-size: 12px; padding: 6px 10px; background: var(--color-background-secondary); border-radius: var(--border-radius-md); display: flex; justify-content: space-between;"><span style="font-family: var(--font-mono); color: var(--color-text-primary);">discount_applied</span><span style="color: var(--color-text-tertiary);">float · NaN=none</span></div>
    <div style="font-size: 12px; padding: 6px 10px; background: var(--color-background-secondary); border-radius: var(--border-radius-md); display: flex; justify-content: space-between;"><span style="font-family: var(--font-mono); color: var(--color-text-primary);">platform</span><span style="color: var(--color-text-tertiary);">iOS/Android/Web</span></div>
  </div>

  <h2 style="font-size: 16px; font-weight: 500; margin: 0 0 10px; color: var(--color-text-primary);">Getting started</h2>
  <div style="background: var(--color-background-secondary); border-radius: var(--border-radius-lg); padding: 1rem 1.25rem; font-family: var(--font-mono); font-size: 13px; color: var(--color-text-secondary); margin-bottom: 24px; line-height: 1.9;">
    <div>pip install numpy pandas jupyter</div>
    <div>git clone https://github.com/J-harshavardhan/swiggy-data-workshop.git</div>
    <div>cd swiggy-data-workshop</div>
    <div>jupyter notebook Swiggy_Workshop.ipynb</div>
  </div>

  <div style="border-top: 0.5px solid var(--color-border-tertiary); padding-top: 14px; font-size: 12px; color: var(--color-text-tertiary);">
    Educational purposes only · Dataset is synthetically generated
  </div>
</div>
